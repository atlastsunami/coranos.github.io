#Camo Banano Example

Lets say I wanted to send private transaction from **ban_1camo** to **ban_3camo**

### ban\_1camo
Seed:    76AB90E5CF854B37150826125418FEA5DD1E34A7CA58E69F18008DC179612783  
Account: ban_1camofhphjj7tyggff9ocb6shkm4ux9z3bf1achgtzyrpfufum16q9w8ryee  
Monkey:  ![ban_1camo](ban_1camo.svg "monKey")

### ban\_3camo and ban\_1mixmkg
Seed:    3E98B56744E0AFBCE8D11F8E41A9D04557AAB3A78899BD4BA2B031FC7210A767  
Account(index 0): ban_3camojbhymtptkwhdngpxj6kg7gfj33dy1ko3yxowqmbo47b8appyqz5cdzf  
Monkey:  ![ban_3camo](ban_3camo.svg "monKey")

Account(index 1): ban_1mixmkgskratqjw3h4eqokyzz5o6uw9hktd1cop6jype55s14571tx1nmcwc
Monkey:  ![ban_1mixmkg](ban_1mixmkg.svg "monKey")

# Create Shared Private Key

First step is to create the shared-secret intermediate private key:

# encrypt Shared Private Key
If I generate a ECDH shared secret I get:
Seed: A468A18F71213BE2B8F7EBD22DE5544186F82F879930E1195E72B069F01A161E
Account: ban_17d9bcxkx5cuxkra4hz991x77tooswkuuhy8eokw3xdhucptzf1fsa1zuzxu
Monkey:  ![ban_17d9.svg](ban_17d9.svg "monKey")

# send funds from ban_1camo to ban_17d9

send your actual funds to the shared private key.
From: ![ban_1camo](ban_1camo.svg "monKey")
To:   ![ban_17d9.svg](ban_17d9.svg "monKey")

# recieve funds at ban_17d9

since ban\_3camo knows she will be recieving funds from ban\_1camo at their shared secret ban\_17d9 they just check the blockchain for any funds at ban\_17d9.  They then move those funds to ban\_1mixmkg, securing them from being taken back by ban\_1camo, but never proving that ban\_3camo was involved in the transaction. ban\_1camo knows that ban\_3camo moved the funds, because only they can know the shared secret.


From:  ![ban_17d9.svg](ban_17d9.svg "monKey")
To:    ![ban_1mixmkg](ban_1mixmkg.svg "monKey")