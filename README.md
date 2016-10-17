# DynAttr - Dynamic Attributes

- author: Ondrej Sika <ondrej@ondrejsika.com>
- license: MIT <https://ondrejsika.com/license/mit.txt>

Dynamic attributes for command line. Written for easy debugging in PyCharm.

## Install

```
git clone git@github.com:ondrejsika.com/dynattr.git
cd dynattr
virtualenv .env
. .env/bin/activate
pip install -r requirements.txt
```

## Run

### Server

```
dynattr --server
```

Open server in browser: <http://localhost:5000>


### Attributes

Example

```
python debugger.py \
    `dynattr --variable script` \
    `dynattr --variable instance` \
    --config=`dynattr --variable config`
```

