# Vagrant virual machine with minikube

Your need install vagrant and virtualbox for up this configuration.

Your need install [vagrant](https://github.com/hashicorp/vagrant-installers/releases/tag/v2.3.4.dev%2Bmain "vagrant") and  [virtualbox](https://www.virtualbox.org/ "virtualbox") for up this configuration. Optional you can use [make](https://www.gnu.org/software/make/ "make").

### Step 1

Download box bento/debian-12 for virtualbox from [vagrantup](https://app.vagrantup.com/bento/boxes/debian-12 "vagrantup").

### Step 2

Clonr this repository: git clone https://github.com/codesshaman/vagrant_docker_with_shared_folder.git

### Step 3

Copy box and go inside the repository folder:

``cp ~/Downloads/735dbb34-5371-4996-8166-f3847a2bfc48 path_to/vagrant_docker_with_shared_folder/debian``

``cd vagrant_docker_with_shared_folder``

### Step 4

Inicialize configuration:

``vagrant box add bento/debian-12 debian``

or with make:

``make build``

### Step 5

Install configuration:

``vagrant up --provider=virtualbox``

or with make:

``make``

### Step 6

Connect:

``ssh vagrant@192.168.58.58``

or with make:

``make connect``

