- **wls --install** 
  - {To install linux}

- **pwd**
  - {print working directory like /home/username}

- **uname -a**
  - {returns the machine architecture i.e. i386 for Intel/AMD platforms}

- **whoami**
  - {returns username}

- **clear**
  - {clear the command window or ctrl + L}

- **mkdir data**
  - {To create directory named data}

- **cd data/**
  - {Going inside folder}

- **vi hello.txt**
  - {vi kind of editor like notepad ++ for linux}
  - {press i and enter}

- **wq** 
  - {press esc and then type this {shift + :}, then use wq{save/quit}}

- **ls**
  - {To check files}

- **q!**
  - {without saving file and return}

- **sudo apt-get install vim**
  - {To install packages sudo{telling my system}, like pip install .. in python}
  - {vim is a package}

- **nano text.txt**
  - {directly can edit}

- **ctrl+shift+v**
- **ctrl+shift+c**

  - {putee dirct select copy right click paste}

- **press d two times**
  - {to delete line}

- **touch foo.txt**
  - {create dummy file}

- **rm file name**
  - {to remove file}

- rm *.txt
  - {to remove all txt files}

- **cat file_name**
  - {to see content inside file}

- **cp old_file_name new_file_name**
  - {to copy content from one file to other}

- **mv old_file new_file**
  - {old file name to new file}

- **cat old_file >> new_file**
  - {append/copy exact content to new file}

- **echo "some_contents" >> file_name**
  - {that some contents will append to old contents}

- **history >> history.txt**
  - {to create/check all our history}

- **~/file_name**
  - {~/ is shortcut for /home/username/}

- **mkdir -p dire/direc/direc**
  - {-p used to create mulitple directories like abc/tst/demo}

<h3><b>cd/ls</b></h3>

- **cd ..**
  - {one directory coming out}

- **cd ../..**
  - {comes to abc path}

- **cd -**
   - {- goes to last directory}

- **ls -lstr**
  - {detail of file/folder {long listing format} comes}

- **ls -a**
  - {shows all files along with hidden files in system}

- **vi .bashrc**
    - {to set path for python /java/enviromnet variable set}

- **source .bashrc**
  - {to execute that enviroment file}

- **.bashrc or .profile or .bashrc_profile**
   - {any one can like this many more}


<h3><b>Hardlink/Softlink</b></h3>

<h4><b>Hardlink</b></h4>

- **ln file_name new_file**
  - {creating hardlink like copy previous data to new file}
  - {if removed rm original file/refrence file still new file there}

<h4><b>Softlink</b></h4>

- **ln -s old_file new_file**
  - {only points file path and inside data if deletes original file/ref file new file also deleted}

<h3><b>alias</b></h3>

- **alias any_name="file_path"**
  - {like if we need to enter to big/long path we can create one alias and give this path name}
  - {it will only alive till close the terminal}
  - {to make it throughout alive/permaanent copy this past and paste/create inside **.bashrc** and source it}

<h3><b>nohup</b></h3>

- **nohub python3 file_name >> new_file_name &**
  - {press enter twice to run this}
  - {Runs specific code or process in background even if system shutdowns/ like ex:code want to run for 4 years like that means not possible to sit for 4 years and monitor thats why we use nohup}

- **top** or **ps** or **ps -aux** or **cat file_name** or **tail -f file_name**
  - {tail to check data/code live}
  - {cat previous printed file}
  - {tail -10 file_name [last ten]}
  - {ps -aux full file details}
  - {to check nohup background code}

- **kill -9 that_folder_number{check in ps}**
  - {to force kill}

- **ps -aux | grep file_name**
  - {to get details of that specific background running file}

- **wget "image_link/download_link"**
  - {to download something to our linux system}

- **df -h**
  - {to check free_space in our disk}

- **du -sh folder_name**
 - {disk_usage summary human_readable/ to check space utilised for that particular directory/file}

- **sudo apt-get install zip**
  - {to install zip}

- **zip -r new_file_name.zip our_folder_name**
  - {to zip our exisiting folder}

- **unzip that_file_name**
  - {to unzip file}

- **tar -czvf new_file_name.tar folder_name**
  - {tar file create/remove, Compress, forceful, verbos_list, Following_list}

- **tar -xzvf file_name**
  - {to untar tar file x-expand, z-forceful}

- **free -m or free -g**
  - {to check ram -m{mb} -g{gb}}

- **sudo sh -c "sync; echo 3 > /proc/sys/vm/drop_caches"**
  - {Not much important/ to remove caches files like gb storage sometimes occupy}

<h3><b>To check words<b></h3>

- **wc file_name**
  - {to check words/total characters}

- **wc -w**
  - {to check words}

- **wc -l**
  - {to check line}

- **wc -c**
  - {to check characters/letters}


<h2><b>SSH{Secure Shell}/SCP{Secure Copy}</b></h2>

<u>to connect other system via ssh</u>

- **ifconfig**
  - {to take ip address number}

- **sudo apt-get install openssh-server**
  - {to install pacakage}

- **ssh ip_address or ssh username@hostname**
  - {to connect to another computer}

- **ssh username or IP Address**

  - {For SSH [use Putty] / winSCP [for SCP]}

- **scp /home/... user2 details**

<h3>Find</h3>

- **find . -name file_name**

- find . -name "*.txt"

- find . -type f -size +10M
  - {to find file greater than 10 Mb}

- find . -mtime -1
  - {one day time frame file}

- touch dummy
  - {to create empty file}

- find . -empty
  - {empty files}

- find . -name "*.tmp" -delete
  - {delete tmp files}

<h2><u>Check difference between grep and find</u><h2>

<table>
  <tr>
    <th>Feature</th>
    <th>'find'</th>
    <th>'grep'</th>
  </tr>
  <tr>
    <td>what it search</td>
    <td>files and directories</td>
    <td>Text inside files</td>
  </tr>
  <tr>
    <td>Used For</td>
    <td>Locatingg filles by name,size,type,etc.,</td>
    <td>searching for matching lines/content</td>
  </tr>
    <tr>
    <td>search level</td>
    <td>works onn filesystem level</td>
    <td>works on file content llevel</td>
  </tr>
    <tr>
    <td>Example</td>
    <td>find . -name "*.log"</td>
    <td>grep "ERROR" log.txt</td>
  </tr>
</table>

<h3>awk</h3>

<h5>table</h5>
<table>
<tr><td>John</td><td>25</td><td>Dev</td></tr>
<tr><td>Mugan</td><td>27</td><td>Designer</td></tr>
<tr><td>Jagam</td><td>30</td><td>finance</td></tr>
</table>

- awk

  - {like excel formulas for linux}

  - {processing columns in text}
  
  - {performing calculations}

  - {extracting and formatiing data from files}

- awk '{print}' file_name

- awk '{print $1}' file_name

- awk '{print $1 $3}' file_name

- awk '$2 > 27 {print $1,$3}' file_name
  - {age > 27}

- awk '{printf "Name: %s| Age: %s | Role: %s\n", $1, $2, $3}' file_name
  - {o/p formatted}

<h4>Mode</h4>
<a href="E:\Linux_learning\image.png">Mode_ref</a>
d r w x r - x r - x

- rw- rw- r--

