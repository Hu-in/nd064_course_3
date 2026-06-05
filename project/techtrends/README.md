<<<<<<< HEAD
# TechTreds Web Application

This is a Flask application that lists the latest articles within the cloud-native ecosystem.

## Run 

To run this application there are 2 steps required:

1. Initialize the database by using the `python init_db.py` command. This will create or overwrite the `database.db` file that is used by the web application.
2.  Run the TechTrends application by using the `python app.py` command. The application is running on port `3111` and you can access it by querying the `http://127.0.0.1:3111/` endpoint.
||||||| empty tree
=======
# nd064_C1
### Cloud Native Fundamentals Scholarship Program Nanodegree Program

**Course Homepage**: https://sites.google.com/udacity.com/suse-cloud-native-foundations/home

**Instructor**: https://github.com/kgamanji

## Quick start

Assuming **Vagrant 2.4.x** and **VirtualBox 7.1.x** are already installed locally,
the snippet below brings up the exercise VM and runs the
[`python-helloworld`](exercises/python-helloworld) Flask sample inside it.

```bash
# 1. Bring up the openSUSE Leap 15.6 VM (uses exercises/Vagrantfile)
cd exercises
vagrant up

# 2. SSH into the VM
vagrant ssh
```

Then, **inside the VM**:

```bash
# 3. Install Python 3.11 and pip
sudo zypper install -y python311 python311-pip

# 4. Install the app's dependencies and start the Flask server
cd /vagrant/python-helloworld
python3.11 -m pip install --user -r requirements.txt
python3.11 app.py
```

The Flask app binds to `0.0.0.0:5000` inside the VM. From a **separate terminal
on your host**, hit it on the VM's host-only IP:

```bash
curl http://192.168.56.4:5000/
# -> Hello World!
```

When you're done:

```bash
exit            # leaves the SSH session
vagrant halt    # run from the host to shut the VM down
```

> The host-only IP `192.168.56.4` is inside VirtualBox 7.x's default-allowed
> range (`192.168.56.0/21`), so no `/etc/vbox/networks.conf` edits are needed.
>>>>>>> 498a476bce1fcda3d57aaa5eac737ce3be9f7630
