# Simple Blockchain Concept in Java
Project ini digunakan untuk membantu dalam menjelaskan mengenai konsep dari blockchain terutama dalam konsep pembentukan block serta mining dalam blockchain. Project ini disusun menggunakan bahasa pemrograman Java. Dalam project ini hanya terdapat 3 class yang terdiri dari class Block, StringUtil dan 1 main class.

Alur yang akan dibahas dalam project ini adalah sebagai berikut. Suatu blockchain akan disimpan dalam bentuk arraylist dan berisikan block-block. Sehingga ketika ingin membuat block dan menambahkannya ke dalam blockchain, maka proses tersebut dapat dilakukan dengan mengeksekusi perintah berikut
```
//Untuk block pertama
blockchain.add(new Block("Hi im the first block", "0"));

//Untuk block selanjutnya
blockchain.add(new Block("Yo im the second block",blockchain.get(blockchain.size()-1).hash));
```
Dengan melihat perintah diatas, maka dapat kita lihat bahwa dalam membentuk suatu block kita memerlukan **data** yang akan kita simpan dan **nilai hash block sebelum**nya.

Proses selanjutnya adalah melakukan validasi atau mining dari block tersebut. Bagaimana proses mining dalam blockchain bekerja?

