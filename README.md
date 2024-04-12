# A Kernel Seedling
TODO: This lab focused on an introduction to linux, and Virtual machines, and the filesystem. The goal was to
determine how many process were currently running on the Virtual machine.

## Building
Below is how I was able to build the program

make 
sudo insmod proc_count.ko 

## Running
To run the program I used the below command
cat /proc/count

The program displayed the total current running processs which was 144.

## Cleaning Up
To clean up the binary I ran

make clean


## Testing
```python
python -m unittest
```
The results from running the unit test were 
...
--------------
Ran 3 tests in 8.063s

OK

Report which kernel release version you tested your module on
(hint: use `uname`, check for options with `man uname`).
It should match release numbers as seen on https://www.kernel.org/.

```shell
uname -r -s -v
```
The Kernel version from the above command 
5.14.8-arch1-1 
