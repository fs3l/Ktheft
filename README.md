# ktheft
Leaked secret keys on the Internet


We publish our dataset of misused keys for external research and development. The GitHub repository is at https://github.com/fs3l/ktheft .

We post the misused-key dataset in three tables as follows: 1) Deposit-transaction table: for each misused secret key $SK$ and its public key $PK$, the table stores a list of deposit transactions, each of which stores attributes like sender account, receiver account (the same as $PK$). 

| SK | PK/to | txIdx [link] | from | value |
| --- | --- | --- | --- | --- | 
| XXX | XXX | XXX [XXX] | XXX | XXX | XXX | 

2) Withdrawal-transaction table: for each misused secret key $SK$ and its public key $PK$, the table stores a list of deposit transactions, each of which stores attributes like sender account (the same as $PK$), receiver account, and etherscan links. 

| SK | PK/from | txIdx | to | value | link |
| --- | --- | --- | --- | --- | --- | 
| XXX | XXX | XXX | XXX | XXX | XXX | XXX | 


3) Leak repositories: for each misused secret key $SK$ and public key $PK$, the table stores a list of repositories, each with an index, the number of forks, stars, and watches, and the link to the repository. 

| SK | PK | repoIdx | forks | stars | watches | link |
| --- | --- | --- | --- | --- | --- | --- |
| XXX | XXX | XXX | XXX | XXX | XXX | XXX | 



4) Leak commit: each row is for a unique combination of misused secret key $SK$ and public key $PK$, a repository index $repoIdx$ and a commit index $ctIdx$. The row stores one value, which is the link to this commit.

| SK | PK | repoIdx | ctIdx | link |
| --- | --- | --- | --- | --- |
| XXX | XXX | XXX | XXX | XXX |
