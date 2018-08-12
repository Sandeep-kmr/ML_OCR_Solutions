# ML_OCR_Solutions

# appconfig.ini

; App configuration
[app]
name        = Welcome
author      = Your Name <you@example.com>
description = a cool new app
keywords    = web2py, python, framework
generator   = Web2py Web Framework

; Host configuration
[host]
names = localhost:*, 127.0.0.1:*, *:*, *

; db configuration
[db]
uri       = sqlite://storage.sqlite
migrate   = true
; ignored for sqlite
pool_size = 10

; smtp address and credentials
[smtp]
server = mailserver.abc.com:25
sender = user1@abc.com
login  = user1:passwd
tls    = false
ssl    = false

; form styling
[forms]
formstyle = bootstrap3_inline
separator =


;XYZ
[XYZ]
client_name = #@START@#Invoice#@@#to#@@#(.*)#@@#(?:c/o|do)#@@#.*
invoice_no = .*#@@#Invoice#@@#Invoice#@@#No#@@#(.*)#@@#Customer#@@#ID#*
