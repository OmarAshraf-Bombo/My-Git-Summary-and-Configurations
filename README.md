# My Git, Github & Terminal Summary, Configurations, Aliases and Files

## How To Use Terminal

cd >> Change Directory >> **cd path_you_need** <br />
mkdir >> Make Directory >> **mkdir folder_name** <br />
rmdir >> Remove Directory >> **rmdir folder_name** <br />
touch >> Create new files >> **touch file_name.extension** <br />
rm >> Remove Files >> **rm file_name.extension** <br />
ls >> List Files and Folders Within the Path >> **ls** <br />



—————————————————————————

## How To Install Git Using HomeBrew on Mac OS

Note >> Mac OS Already has git installed by Default, but HomeBrew git is better than Stock <br />

1. nstall HomeBrew First From This Link >> https://brew.sh/ <br />
2. Check if There is any updates by typing >> **brew update** or **brew upgrade** <br />
3. Install git by typing >> **brew install git** <br />
4. Check version by typing >> **git -\-version** <br />


—————————————————————————


## How To Use Git

#### Git Initialization

Change Directory to the Path of the Project <br />
Type >> **git init** <br />

—————————————————————————

#### Git Configurations

- **Git config -\-global user.name “Omar Ashraf"** <br />
- **Git config -\-global user.mail “omar_ashraf_93@hotmail.com”** <br />
- **Git config -\-global user.author “Omar Ashraf”** <br />


—————————————————————————

#### Check Repo Status

Type >> **git status** <br />

—————————————————————————

#### Adding Files to Staging Area and Unstaging Files

Type >> **git add .** Or **git add *** or **git add file_name** <br />
Type >> **git reset .** Or **git reset *** or **git reset file_name** <br />

—————————————————————————

#### Committing to Local Repo

Type >> **git commit -m “Your Commit Message”** <br />

—————————————————————————

#### Git Log

Type >> **git log**  <br />
Or <br />
Type >> **git log -\-oneline** <br />


—————————————————————————

#### Undoing ( Checkout, Revert & Reset )

##### ##### Checkout Commit
Type >> **git checkout COMMIT_ID** <br />
>> It Will Only Show You What The Code Was Like at This Commit ( Read Only ) <br />

##### ##### Revert Commit
Type >> **git revert COMMIT_ID** <br />
>> It Will Revert The Commit ID You Passed to it by Adding One More Commit With the Revert. <br />

##### ##### Reset Commit
Type >> **git reset COMMIT_ID -\-hard** <br />
>> It Will Reset the HEAD to The Commit ID You Passed to it & Remove all the Commits after it as it never happened. <br />


—————————————————————————

#### BranchesBranches

##### ##### Create New Branch
Type >> **git branch branch_name** <br />

##### ##### Checkout to the branch
Type >> **git checkout branch_name** <br />

##### ##### Checkout to the master
Type >> **git checkout master** <br />

##### ##### Create branch & checkout in one command
Type >> **git checkout -b branch_name** <br />

##### ##### Show All Branches
Type >> **git branch** <br />

##### ##### Delete branch
Type >> **git branch -d branch_name** >> Only Works if Branch is Megred <br />
Type >> **git branch -D branch_name** >> Works Even if Branch is Not Merged <br />

##### ##### Merging branches With Master
Note: You Have to be on the Master to be able to merge <br />
Type >> **git checkout master** <br />
Type >> **git merge branch_name** <br />


—————————————————————————

#### Git Clone

Type >> **git clone URL.git** <br />


—————————————————————————

#### Generate & Test SSH Key ID

1- Type >> **ssh-keygen -t rsa -b 4096 “omar_ashraf_93@hotmail.com”** <br />
Or Type >> **ssh-keygen -o -t rsa -c “omar_ashraf_93@hotmail.com”** <br />
2- Enter File Path: **Enter** <br />
3- Enter **Password** <br />
4- Re-Enter **Password** <br />
5- **cat ~/Path/Path/id_rsa.pub** <br />
6- Copy The ID Value Starts with ssh-rsa <br />
7- Open Github Settings > SSH & GPG Keys <br />
8- New SSH Key <br />
9- Enter The Copied ID Value & Give it a Proper Name <br />
10- **Type ssh -T git@github.com ** <br />
11- Enter **Password** <br />
> DONE (AUTHENTICATED) <br />

—————————————————————————

#### Change SSH Key ID Password

1- Type >> **ssh-keygen -p** <br />
2- Enter File Path: **Enter** <br />
3- Type **Old Password** <br />
4- Type **New Password** <br />
5- Retype **New Password** <br />
> DONE

—————————————————————————

#### Aliases
Type >> **git config —global alias.(Shortcut) (Command)** <br />
Example >> **git config —global alias.st status** <br />

>> Now git status = git st <br />


—————————————————————————

#### Push To Remote Repo
Type >> **git push origin master** <br />
Or to push a branch <br />
Type >> **git push origin branch_name** <br />




# My Git Configuration Files & Aliases
- (.gitconfig) >> Git Configurations <br />
- (.gitignore) >> Ignoring Files to be Added or Committed <br />
- (.zshrc) >> Adding Branch Name to End of Line in Terminal <br />

- Note >> If These Files are not created in the System By Default <br />
- Type >> **touch ~/.gitconfig** <br />
- Type >> **touch ~/. zshrc** <br />
- Type >> **touch project_path/.gitignore** <br />


