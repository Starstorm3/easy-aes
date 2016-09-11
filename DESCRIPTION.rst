easy-aes
========

easy-aes is an ultra-lightweight, pure-python library for doing AES
encryption. It draws heavily on the popular crypto library, simplifying
AES encryption and decryption of files to a single function each.

Usage
-----

Simple usage follows this pattern:

.. code-block:: python

  import easy-aes
  encrypt_me = "my_transcript.pdf"
  output_file = easy-aes.encrypt_file(encrypt_me)

output_file is a string with the new file name.

WARNING: IF YOU FORGET YOUR PASSWORD AND DELETE
THE ORIGINAL DATA, YOUR FILE WILL NOT BE ABLE TO BE RETRIEVED!

.. code-block:: python

  import easy-aes
  encrypted_file = "my_encrypted_filename.aes"
  binary_data = easy-aes.decrypt_file(encrypted_file)
  with open('my_new_file.aaa','wb') as new_file:
    new_file.write(decrypted_data)

decrypt_file returns a Python object containing 
the now-decrypted data.

Installation
------------

easy-aes works Python 3.3+. To install it,
use:

.. code-block:: bash

    $ pip install easy-aes

0.1
~~~

Released on September 10, 2016