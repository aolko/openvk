# OpenVK

### Mirrored from [github](https://github.com/openvk/openvk)

A failed kiddie project at cloning the classic vkontakte.ru, was pentested @ 2-ch and successfully broken.

## Security risks

Contains quite a few security risks, including, but not limited to:

* Mysql injection possibilities
* XSS possibilities
* Missing and/or broken field validation
 

## Architectural flaws

* Currently consists as a mess of not formatted/badly formatted php files
* No code structure (so far)
* No templating engine (which would simplify some things) (which also includes the fact that templates and code are squished together)
* No prepared statements in sql connections/queries or an sql middleware (like notorm/redbean or meekrodb)


## Flaws?

* This project does not rely on Composer packages
* ...and on PSR standards
* This project has quite bad routing (every route defined thru .htaccess) and could use a router instead
* .htaccess itself contains quite a bunch of php flags and php options related to debugging and specifying the log location
 

## Improving this project

If you want to improve this project, please fork it. In this repository it is presented AS IS.
