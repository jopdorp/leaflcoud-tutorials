# Log in to your instance

This tutorial will show you how to log in to your instance

Open your terminal and enter the following:

``` shell
ssh [os_name]@[Instance Public IP Address]
```

So, for example: 

``` shell
ssh centos@[Public IP]
```

Enter your username and password

You have now logged in to your instance

## Log in using an imported Key Pair

To log into your instance using a specific SSH key, type the following in your terminal:

``` shell
ssh -i .ssh/id_rsa [os_name]@[Public IP]
```

## Log in using a generated Key Pair

To log into your instance using a generated key, download your keypair file (.pem) locally

Navigate to the downloaded .pem file using your terminal

First secure your key file by entering:

``` shell
chmod 400 [name of your key pair].pem
```

Now log in using the following command: 

``` shell
ssh -i [key pair name].pem [os_name]@[Public IP]
```

You have logged in to your instance
