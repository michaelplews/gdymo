# gdymo
gdymo is a simple wrapper around [ppl](http://ppladdressbook.org/) and [gLabels](http://glabels.org/) that makes it easy to pick users from your existing ppl address book and create shipping labels for them as `.pdf` files. These can then be easily printed to a Dymo label printer. This is also my first bash project, and a chance to experiment with bash programming.

## Installation

### Ubuntu

```bash
git clone https://github.com/michaelplews/gdymo.git
cd gdymo
sudo chmod +x gdymo
sudo ln -s gdymo /usr/local/bin 
```

## Usage

```bash
Usage: <OPTIONS>
-i  id of ppl entry
-a  address reference of ppl entry
-t  <US|UK> label format
```

### Example:

```bash
gdymo -i president -a home
```

Results in:

![president label](examples/president.png)

## gLabels Templates
I am using template files that fit my Dymo printer, however these template files may need to be adjusted to fit your needs. Alternatively, you can rearrange the template files provided in this repo to create additional 'types' and specify the type by adding options to the `-t` option. 
