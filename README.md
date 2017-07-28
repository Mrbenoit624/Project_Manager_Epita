# README


 You can contact if you have some suggestion or bug to report.
## GENERAL INFO


  Project: Project_Manager_Epita</br>
  Contributors: forget_c</br>
  License: GNU General Public License v3.0</br>
  Version: v1.5</br>
  Date: 12-21-16</br>
  </br>
  Epita 2019 - ING 1
## GOAL


  The goal of this project is to generate automatically REDME TODO and the
  architecture in order to help developers to work quickly.
  An editor of TODO is also integrate.
## USAGE


  You can put the pre-commit file in your hook if you want to use at each commit
  but you con also use it just like a script.</br>

*Usage: ./pre-commit <font color="red">[-ut]</font> [-c] [-a] [-r] [-t file] [-init file] [-conf file]*

* if you use:</br>
    ./pre-commit</br>
    all functionalities should be used but not forced if it's exist it must not
    executed

* if you use:</br>
    ./pre-commit -ut</br>
    you launch the interactive editor of TODO
    use <code>\<enter\></code> to change a field

* if you use:</br>
    ./pre-commit -c</br>
    a little correction of your coding style must be launch  (a better
        correction with clangformat, don' correct 25 lines in a functions)

* if you use:</br>
    ./pre-commit -a</br>
    a AUTHORS must be generated

* if you use:</br>
    ./pre-commit -r</br>
    a README like this must be generated but you can specified some field in
    your config file {VERSION, DATE, PROJECT, LICENSE, INFO}

* if you use:</br>
    ./pre-commit -t file</br>
    a TODO is generated thanks to the file give in parameter
    the file supported is ACU 2017 subject


* if you use:</br>
    ./pre-commit -init file</br>
    the architecture is generated thanks to the file give in parameter
    the file supported is ACU 2017 subject

* if you use:</br>
    ./pre-commit -t file</br>
    a conf file is generated thanks to the file give in parameter
    the file supported is ACU 2017 subject
### GLOBAL VARIABLE
    in the head of the script you can modify some variable

    login: list of the login in the following format</br>
      login="login_x login_y"

    ignore_files: list of the file contains the files or directory should not
      be corrected by the corrector of the coding style.

    path_subject: the path to the subject if you use the command without
    parameter

    step: list of the step in the todo in the following format</br>
      step=("STEP 1" "STEP 2")

    config_file: the path where the config file is

    clangformat: the path of the clang format file to have a better correction
    let an empty string if you don't have clang-format
### CONFIG FILE
    The format is the following one:</br>
      VAR=VALUE



## CHANGELOG
