# Basic commands of Anaconda

Date: 28th Feb 2021

System: Mac OS



## Content

- use command to activate the bash so that we can use command s of anaconda (If you use window you may not to do this)

  ```
  $ source ~/.bash_profile
  ```

- check the version of anaconda

  ```
  $ conda --version
  ```

- update anaconda

  ```
  $ conda update conda
  ```

- If you are in China, the internet may be very slow for the updating, so you can use the follow command to change your update source bofore you update anaconda:

  ```
  $ conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
  
  $ conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main/
  
  $ conda config --set show_channel_urls yes
  ```

- Check the installed moduels and deependencies. 

  ```$ conda list```

- Create a new python environment

  ```
  $ conda create --name envName
  ```

  envName is the name of environment

- Create a new python environment with particular python version

  ```
  $ conda create -n envName python=3.7
  ```

- Create a new python environment with particular modules and dependencies

  ```
  $ conda create -n envName scipy
  ```

- Create a new python environment with particular modules with a particular version

  ```
  $ conda create -n envName scipy=0.15.0
  ```

- Duplicate an environment

  ```
  $ conda create --name cloneEnv --clone envName
  ```

- Verify the duplication

  ```
  $ conda info --envs
  ```

- Activate an environment

  ```
  $ source activate envName
  ```

- Quit from an environment

  ```
  $ source deactivate
  ```

- Delete an environment

  ```
  $ conda remove --name envName --all
  ```

- Check the list of a particular environments
  ```
  $ conda info --envs
  ```

  or

  ```
  $ conda env list
  ```

- Check the installed modules and dependencies of a particular environment

  ```
  $ conda list -n envName
  ```

- Search module

  ```
  $ conda search moduleName
  ```

- Install module

  ```
  $ conda install moduleName
  ```

- Update module

  ```
  $ conda update moduleName
  ```

- Remove module

  ```
  $ conda remove moduleName
  ```

- Install module to a particular environment

  ```
  $ conda install -n envName moduleName
  ```

  