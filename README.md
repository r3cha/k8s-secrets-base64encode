# k8s-secrets-base64encode
This is Ruby script that parse you k8s secrets config base64encode values and save that you’ll able apply it with kubctl


## how to use it

Copy to you, run it with filepath arguments like

`bin/encode_k8s_secrets path-to-file/secrets-filename.yml`  

In my case ` bin/encode_k8s_secrets deploy/k8s/staging/.secrets.yml`  
It will create new file with path `deploy/k8s/staging/.secrets-base64.yml` where all env value will be base64

Also can pass multimple file paths `bin/encode_k8s_secrets filepath-one.yml filepath-two.yml` 
