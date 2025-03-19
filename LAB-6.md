## LAB-6 Create the operator1 user and confirm that it exists in the system. Set the password for operator1. Create the additional operator2 and operator3 users. Set their passwords as well. Run the usermod -c command to update the comments of the operator1 user account. Remove the operator3 user from the system.


### Step 1 - Create a new user

```
sudo useradd operator1
```

### Step 2 - Setting the password for operator1

```
sudo passwd operator1
```

## Step 3 - Create two more users operator2 & operator3

```
sudo useradd operator2
sudo useradd operator3
```

### Step 4 - Setting the passwords for operator2 & operator3

```
sudo useradd operator2
sudo useradd operator3
```


### Step 5 - Set the comments of the user operator 1

```
sudo usermod -c "Doing lab 12" operator1
getent passwd operator1
```

### Step 6 - Remove operator 3 and view the updated users list

```
sudo userdel operator3
getent passwd
```

![Screenshot 2025-03-19 183048](https://github.com/user-attachments/assets/26345d23-8f91-4695-b63b-ec25aa31f005)
![Screenshot 2025-03-19 183057](https://github.com/user-attachments/assets/e19761b8-ddca-497b-af12-02b6605cd4a8)
