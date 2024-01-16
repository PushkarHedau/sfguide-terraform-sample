# sfguide-terraform-sample
$ mkdir sfguide-terraform-sample && cd sfguide-terraform-sample
$ echo "# sfguide-terraform-sample" >> README.md
$ git init
$ git add README.md
$ git commit -m "first commit"
$ git branch -M main
$ git remote add origin git@github.com:PushkarHedau/sfguide-terraform-sample.git
$ git push -u origin main

$ cd ~/.ssh
$ openssl genrsa 2048 | openssl pkcs8 -topk8 -inform PEM -out snowflake_tf_snow_key.p8 -nocrypt
$ openssl rsa -in snowflake_tf_snow_key.p8 -pubout -out snowflake_tf_snow_key.pub
