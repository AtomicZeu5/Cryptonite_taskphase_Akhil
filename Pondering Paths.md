# Pondering Paths

This module will teach you the basics of Linux file paths! A path from the filesystem's root starts with / (that is, the root of the filesystem), and describes the set of directories that must be descended into to find the file.

## 2.1 The Root

  In this challenge, we had to invoke the pwn program using its absolute path, and we achieved this by using the `/` command. hence, we execute /pwn to get the flag.


  ### Flag
  ```
  pwn.college{EsLlv5qGEozMbT47a5uu9O2S_v1.dhzN5QDL3cTN0czW}
```

## 2.2 Program and absolute paths

  In this challenge, we had to execute `run` , which is in the `challenge` directory. However, we had to invoke this by using an absolute path which can be done with `/`. Hence, we run the command /challenge/run to get the flag.

  ### Flag
  ```
   pwn.college{4eHhkMUUr9OUV-EgZN0AGDgfsbD.dVDN1QDL3cTN0czW}
```
## 2.3 Position thy self

  In this challenge, we learnt how to use the `cd` command to change directories. We have to execute /challenge/run from an unknown directory. First, we execute /challenge/run in the home directory. It gives an error and reveals the directory from which we must execute it. In my case, it was /var/log. I changed directory by typing `cd /var/log`, we then executed `/challenge/run` to get the flag.

  ### Flag
  ```
   pwn.college{8linXITSQbwIFVi_mqBjGt4Fv7B.dZDN1QDL3cTN0czW}
```

 ## 2.4 Position elsewhere

  Same process as 2.3, tried trial and error until I got the correct directory to change to, then executed `/challenge/run`.

  ### Flag
  ```
    pwn.college{8linXITSQbwIFVi_mqBjGt4Fv7B.dZDN1QDL3cTN0czW}
```

## 2.5 Position yet elsewhere

   Same process as 2.3, tried trial and error until I got the correct directory to change to, then executed `/challenge/run`.

   ### Flag
   ```
   pwn.college{sHOXAwmJpuvqFkEda3VEzn07fcu.dhDN1QDL3cTN0czW}
```

## 2.6 implicit relative paths, from /

  This challenge introduces us to relative paths. These are basically relative to the current directory. In this challenge, we are asked to run `/challenge/run` from a relative path, while having a current directory of `/`. This can be achieved by `cd /`. Then we type `challenge/run` to get the flag.

  ### Flag
  ```
pwn.college{4upOT1XfJ7HA5bmuXcKg8r5atpM.dlDN1QDL3cTN0czW}
```

## 2.7 Explicit relative paths, from /

Previously, your relative path was "naked": it directly specified the directory to descend into from the current directory. In this level, we're going to explore more explicit relative paths. If we try to execute `/challenge/run` from the directory `/` normally, it doesn't work. We have to use a relative path while being in the `/` directory, hence executing `./challenge/run` from `/` gives us the flag

### Flag
```
pwn.college{Iiwst5NNI4ErXVGt6O-6P2OmwkF.dBTN1QDL3cTN0czW}
```

## 2.8 implicit relative path

In this challenge, we are required to run `./run` from `/challenge` directory.

### Flag
```
pwn.college{Ul8-kmkJLH5E3y2xzTKh_PIiaTO.dFTN1QDL3cTN0czW}
```
## 2.9 Home sweet home

In this challenge, we use the command `echo` to display a certain argument or file. First, we use `echo LOOK: ~` as shown in the tutorial. This displays `LOOK: /home/hacker` to us. One of the restrictions is that the file has to be less than 3 characters. So, we need to get the flag from the home directory through a file which is less than 3 characters so I named it a. Then I executed `/challenge/run ~/a` since only the leading ~ is expanded. This gave me the flag

### Flag
```
pwn.college{IrRq6qUnx4nk2fKJgBjkbxkb9g9.dNzM4QDL3cTN0czW}
```







  
