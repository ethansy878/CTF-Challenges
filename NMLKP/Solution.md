1. Open the program and begin searching. 

2. As the user searches, some of the names will appear to be corrupted. These are messages encoded in Base64. 
    > The user can either figure this out themselves, or look at the extra-long transmission that appears when entering "NMLKP" as a search query. This transmission has an equals sign at the end, a common sign of Base64. Also, after 50 searches, NMLKP will make a comment to search for it at the party, guiding users to this hint.

3. Record each corrupted entry and decode it using a Base64 decoder. These "pieces of evidence" give the order of the names.

4. Figure out which names have been replaced by these messages.
    > The user can either be clever with their searches and deduce the names themselves, or return to the "NMLKP" transmission to get a hint. Decoding the transmission twice returns a link to a Social Security Top 100 Names website. The first 50 boys and girls are all the people in the party. This will make deducing the names easier!

5. Put the names in order, wrap in broncoctf{}, submit!

The flag is:
broncoctf{MichaelStephanieAmyDennisJennifer}


Note: Not all steps are necessary to complete the challenge. The hints from searching "NMLKP" help, but are not mandatory.
A user can also try reversing the program and see what they find doing so. The order of names is stored in a regular char[][] array in the correct order and with no obfuscation. They may be able to find the names and the order this way.