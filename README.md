# My Git, Github & Terminal Summary, Configurations, Aliases and Files

## How To Use Terminal

cd >> Change Directory >> **cd path_you_need**
mkdir >> Make Directory >> **mkdir folder_name**
rmdir >> Remove Directory >> **rmdir folder_name**
touch >> Create new files >> **touch file_name.extension**
rm >> Remove Files >> **rm file_name.extension**
ls >> List Files and Folders Within the Path >> **ls**



—————————————————————————

## How To Install Git Using HomeBrew on Mac OS

Note >> Mac OS Already has git installed by Default, but HomeBrew git is better than Stock

1. nstall HomeBrew First From This Link >> https://brew.sh/
2. Check if There is any updates by typing >> **brew update** or **brew upgrade**
3. Install git by typing >> **brew install git**
4. Check version by typing >> **git -\-version**


—————————————————————————


## How To Use Git

#### Git Initialization

Change Directory to the Path of the Project
Type >> **git init**

—————————————————————————

#### Git Configurations

- **Git config -\-global user.name “Omar Ashraf"**
- **Git config -\-global user.mail “omar_ashraf_93@hotmail.com”**
- **Git config -\-global user.author “Omar Ashraf”**


—————————————————————————

#### Check Repo Status

Type >> **git status**

—————————————————————————

#### Adding Files to Staging Area and Unstaging Files

Type >> **git add .** Or **git add *** or **git add file_name**
Type >> **git reset .** Or **git reset *** or **git reset file_name**

—————————————————————————

#### Committing to Local Repo

Type >> **git commit -m “Your Commit Message”**

—————————————————————————

#### Git Log

Type >> **git log** 
Or
Type >> **git log -\-oneline**


—————————————————————————

#### Undoing ( Checkout, Revert & Reset )

##### ##### Checkout Commit
Type >> **git checkout COMMIT_ID**
>> It Will Only Show You What The Code Was Like at This Commit ( Read Only )

##### ##### Revert Commit
Type >> **git revert COMMIT_ID**
>> It Will Revert The Commit ID You Passed to it by Adding One More Commit With the Revert.

##### ##### Reset Commit
Type >> **git reset COMMIT_ID -\-hard**
>> It Will Reset the HEAD to The Commit ID You Passed to it & Remove all the Commits after it as it never happened.


—————————————————————————

#### BranchesBranches

##### ##### Create New Branch
Type >> **git branch branch_name**

##### ##### Checkout to the branch
Type >> **git checkout branch_name**

##### ##### Checkout to the master
Type >> **git checkout master**

##### ##### Create branch & checkout in one command
Type >> **git checkout -b branch_name**

##### ##### Show All Branches
Type >> **git branch**

##### ##### Delete branch
Type >> **git branch -d branch_name** >> Only Works if Branch is Megred
Type >> **git branch -D branch_name** >> Works Even if Branch is Not Merged

##### ##### Merging branches With Master
Note: You Have to be on the Master to be able to merge
Type >> **git checkout master**
Type >> **git merge branch_name**


—————————————————————————

#### Git Clone

Type >> **git clone URL.git**


—————————————————————————

#### Generate & Test SSH Key ID

1- Type >> **ssh-keygen -t rsa -b 4096 “omar_ashraf_93@hotmail.com”**
Or Type >> **ssh-keygen -o -t rsa -c “omar_ashraf_93@hotmail.com”**
2- Enter File Path: **Enter**
3- Enter **Password**
4- Re-Enter **Password**
5- **cat ~/Path/Path/id_rsa.pub**
6- Copy The ID Value Starts with ssh-rsa
7- Open Github Settings > SSH & GPG Keys
8- New SSH Key
9- Enter The Copied ID Value & Give it a Proper Name
10- **Type ssh -T git@github.com **
11- Enter **Password**
> DONE (AUTHENTICATED)

—————————————————————————

#### Change SSH Key ID Password

1- Type >> **ssh-keygen -p**
2- Enter File Path: **Enter**
3- Type **Old Password**
4- Type **New Password**
5- Retype **New Password**
> DONE

—————————————————————————

#### Aliases
Type >> **git config —global alias.(Shortcut) (Command)**
Example >> **git config —global alias.st status**

>> Now git status = git st


—————————————————————————

#### Push To Remote Repo
Type >> **git push origin master**
Or to push a branch
Type >> **git push origin branch_name**




# My Git Configuration Files & Aliases
- (.gitconfig) >> Git Configurations
- (.gitignore) >> Ignoring Files to be Added or Committed
- (.zshrc) >> Adding Branch Name to End of Line in Terminal

- Note >> If These Files are not created in the System By Default
- Type >> **touch ~/.gitconfig**
- Type >> **touch ~/. zshrc**
- Type >> **touch project_path/.gitignore**


