## Cloud crushing with driven turbulence
Codes for driven turbulence in CC setup (with PLUTOv4.4p2)
---

#### 🏃 Initialization

* Compile Pluto with its dependencies and create the executable `./pluto`
  ```
  make -j$(nproc) && make clean 
  ```
* Use the provided [slurm jobscript](./hydro-rps/slurm-script) to run parallelly on your supercomputer
  ```
  sbatch slurm-script
  
#### __:bookmark:Important Files:__ ##
> - [init.c](./turb/init.c) &rarr; problem initialization and on-the-fly analysis
> - [pluto.ini](./turb/) &rarr; input parameters
> - [definitions.h](./turb/definitions.h) &rarr; problem / solver settings
> - [userdef_output.c](./turb/userdef_output.c) &rarr; script for user-defined outputs

### 🧑‍💻 Developers

[🔗](https://github.com/RitaliG) Ritali Ghosh
