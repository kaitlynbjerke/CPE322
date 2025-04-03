# Lab 10 - Blockchain
## Kaitlyn Bjerke
### I pledge my honor that I have abided by the Stevens honor system - *Kaitlyn Bjerke*
---
**Description:** In this lab, we learned about hash values and how to mine blocks.

**Prelab tasks:** For this lab, we are going to use two terminals, so I opened up both terminals and copied over the necessary repository: `git clone https://github.com/satwikkansal/python_blockchain_app.git`

hash_value.py
---
run `python hash_value.py` twice:
![hash](https://github.com/kaitlynbjerke/Images/blob/main/hash.png)

As seen above, the values for the numbers remain constant. However, the values for the strings (vowels/person) change. For this lab, we are utilizing [PYTHONHASHSEED](https://docs.python.org/3/using/cmdline.html#envvar-PYTHONHASHSEED), which specifies that "a random value is used to seed the hashes of str and bytes objects." That is why the hashes for the strings are random -- the random value resets each time the function is called.

snakecoin.py
---
![snakeCoin](https://github.com/kaitlynbjerke/Images/blob/main/snakecoin.png)

This function prints out 20 instances of a block getting added to the blockchain, alone with the block's respective hash.

snakecoin-server-full-code.py
---
In one terminal, I ran the following code, which prints out the url where you can view the resultant webpage.

![snakeCoinFull](https://github.com/kaitlynbjerke/Images/blob/main/snakeCoinFull.png)

On the other terminal, I utilized **curl,** which is a method of transferring data. This allowed me to "mine" the Snake Coins.

![curl](https://github.com/kaitlynbjerke/Images/blob/main/curl.png)

Below, you can see the output of the webpage, which simply states "SnakeCoin Server"

![snakeCoinServer](https://github.com/kaitlynbjerke/Images/blob/main/snakeCoinServer.png)

The second terminal leads to a separate webpage, which has a very similar display to the output in the terminal beneath the function call.

![8000mine](https://github.com/kaitlynbjerke/Images/blob/main/8000mine.png)

node_server.py
---
In the first terminal, I ran `node_server.py`, which displays a link to a webpage that the script is runnnig on.

![nodeserver](https://github.com/kaitlynbjerke/Images/blob/main/node_server.png)

On the other terminal, I ran `run_app.py`, allowing both webpages to run simulaneously.

![runapp](https://github.com/kaitlynbjerke/Images/blob/main/runApp.png)

After opening http://127.0.0.1:5000/, I was probed to create a post. Thus, I entered "hello", put in my name, and hit "post."

![yournet](https://github.com/kaitlynbjerke/Images/blob/main/yourNet.png)

This brough me to a secondary site, which output "Block #1 is mined." After further experimentation, I realized that each post corresponded to one extra block mined.

![mined](https://github.com/kaitlynbjerke/Images/blob/main/mined.png)

Once returning to the main webpage, I pressed **Resync,** which allowed the new post to appear.

![post](https://github.com/kaitlynbjerke/Images/blob/main/post.png)
