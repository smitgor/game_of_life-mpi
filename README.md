# game_of_life-mpi

## login to your cluster
```
starcluster sshmaster <clustername>
```

## change user to admin
```
su - <admin user name>
```

save your file in admin user

## compile the code
```
mpicc gameoflife.c -std=c99 -o gameoflife
```

## Run the exe file
```
mpirun -n 4 -host master,node001,node002,node003 ./gameoflife
```
