                                   Decrypting 6-Round-DES


For solving this, we used DIFFERENTIAL CRYPTANALYSIS. In order to break the six rounds of the given DES, 
we do a chosen plaintext attack . We need a 4 round characteristic to break a 6-round DES which is obtained 
after 4 rounds of the 5-round characteristic discussed in lecture 7. The differential iterative characteristic
starts at 405c0000 04000000 and after 4 rounds gives the differential 00540000 04000000
with probability = ¼ *5/128 * ¼ * 5/128 = 0.000381 . Thus we need approximately 20/0.000381
= 52000 chosen input pairs to get assurity of finding the right key. 
