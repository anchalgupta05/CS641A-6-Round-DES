# CS641A-6-Round-DES

Inputs generate folder - generates 64 bits of binary string using random_inputs.cpp and stores then in random.txt.
Then generates pairs of input plaintext using random_inputs_xor.cpp and stores them in input_random.txt.

get_outputs.sh has the script that stores all the commands that we will send to the ssh server.
In order to grep the encrypted text, we first store all the terminal output in ssh_outputs.log then the encrypted text is grep from this file and stored in freq_outputs.txt. 
get_outputs.sh redirected the output to ssh_outputs.log directly and the grepping part was done using the report_freq.py.

The get_outputs.sh was made from the script.py with the help of input_random.txt that we had generated above.
Delete ssh_output.log before running the get_outputs.sh since it appends and delete freq_outputs.txt before running the report_freq.py (same reason).
