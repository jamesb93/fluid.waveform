# Fluid Waveform Build Package 

The bits needed to build the Max-JS compatible version of fav.js, assemble the ingredients for including in a Max package. 

## TODO 

* Finish decoupling from embedded fav.js and instead pull as NPM module from GH

> The idea has been not to touch fav at all, but only with partial success so far. So, go through and peel out changes into freestanding code or patches so that we can stay in sync with upstream

* Document what Babel is doing: tl;dr converting ES6 to Max's older and somewhat idiosyncratic JS. The horrible bit is that the `requires` stuff ends up needing extra massaging with a custom plugin 

## Go 

Run 
```
npm run build 
```
and everything you need to use the object in Max should be in the `max_package` subtree 
