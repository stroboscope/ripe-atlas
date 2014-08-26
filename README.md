# ripe-atlas


ripe-atlas is a minimalistic API wrapper for the [RIPE Atlas](https://atlas.ripe.net) API. It is written entirely in Ruby.

## Usage

First, you should require the gem:
```ruby
require 'ripe-atlas'
```

Then you can get Atlas probes by specifiying parameters. I.e.:
```ruby
Atlas.get_probe({:id => 333})
```

This should give you an array with the Atlas probes. Since we specified the exact ID of the probe, 
we should get just one probe object in the array. It could look like this:
```
[#<Atlas::Probe:0x000000022db840 @address_v4="126.15.248.61", @address_v6="2400:2410:20c0:111:220:4aff:fec8:242e", 
@asn_v4=17676, @asn_v6=17676, @country_code="JP", @id=333, @is_anchor=false, @is_public=true, @latitude=35.6585, 
@longitude=139.7485, @prefix_v4="126.15.0.0/16", @prefix_v6="2400:2000::/20", @status=1, @status_name="Connected", @status_since=1408477001>] 
```

##TODO
* Add measurement and probe-participation-request
* Publish gem on RubyGems.org
* Clean up code. 


## Donate

If you would like to support me, you can buy me a bottle of Club Mate via GitTip:

<a href="https://www.gittip.com/EddyShure/">
  <img alt="Support via Gittip" src="https://rawgithub.com/twolfson/gittip-badge/0.2.0/dist/gittip.png"/>
</a>
