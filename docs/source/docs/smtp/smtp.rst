*************
SMTP
*************

Linux
=========

sendmail
--------
To test whether smtp is working:

see https://www.linuxbabe.com/redhat/run-your-own-email-server-centos-postfix-smtp-server

.. code:: bash

    echo "test email" | sendmail [sabine.maennel@liip.ch](mailto:sabine.maennel@liip.ch)


.. code:: bash

    cd /var/log
    cat maillogs* | grep ogd@liip.ch




Python
=======

see https://docs.python.org/2/library/smtplib.html

.. code:: python

    import smtplib
    server = smtplib.SMTP('localhost')
    server.set_debuglevel(1)
    server.sendmail('no-reply@opendata.swiss', 'sabine.maennel@liip.ch', 'hello')
    server.quit()