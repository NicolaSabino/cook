# The cooking file system
 
Even if we live in digital modern times, food is still treated analogically.

To obtain infos about a product we have to read the label squashed in few squared centimeters. The expiration date is just printed on the box and it makes tricky to add more details on what we are eating!

There are thousand of food bloggers, sharing their receipts with videos, textual posts, short IG stories but there is a lack of a standard way to communicate effectively these information. 

Imagine to approach a video receipt from a food blog, download a file and being able to add it to your digital cookbook. Being able to customize the script, add your personal touch and share it with your a friend via chat, email, bluetooth or even publish it on social networks.

The main idea is to propose a standard file extension system for food, ingredients and receipts.

In the same way the `.pdf` extension is associated nowadays to documents and books, `.png` for pictures and `.zip` for archives, we would like to propose a standard file format, `.cook` based on JSON technology, to easily share food information and create a reliable, open-source and easy-to-use tool to built services upon it.

## Applicative scenario of a .cook file

### The file creation
Let's imagine that the famous Chef Rossi from Rome is finalizing his recipe of Amatriciana pasta for his restaurant in Trastevere. 

In order to enrich the offer of his shop and make it more appealing for clients he decide to attach a qr code on the menu with a downloadable digital version of the recipe, `The traditional amatriciana by Chef Rosssi.cook` created via an online recipes editor. In this way clients can try to reproduce themselves the recipe at home.

Such file contains some special indications about the cheese used for the recepie, a Pecorino DOP, with a shop link to an affiliate cheese maker.

### The spread and customization
Amy, an American food blogger decided to visit Chef Rossi's restaurant and to try his special Amatriciana dish. She scan the qr code downloading the recipe in her cookbook application. Reached her apartment in the states she decided to customize the original version from Chef Rossi, replacing the *Pecorino* cheese with a dried local cheese easier to find in America. Furthermore she wants to replace the *spaghetti* pasta, with *mezze maniche*.

She will perform all this changes in the cookbook application and publish on her food blog the file `Reinterpreted Amatriciana.cook` . **The file will contain the both Amy's and the original version from Chef Rossi** in a sort of timeline.

### Online shops
Mark, a banking employer with passion of Italian dishes, is Amy's fan and decide to download her recipe from the blog. He will use a new feature from his favorite online food shop. Simply uploading the .cook file from amy he can select the missing groceries to buy and order a deliver to his apartment for a dinner with some colleagues.

### Peer to Peer recipe sharing
The dinner is a success and Susy, Mark's boss is asking for the recipe. Mark open his cookbook app and share such file with Susy via Bluetooth.