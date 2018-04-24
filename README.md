# Cybersecurity-Week-7

Time spent: 3 days spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) XSS 
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.0
    - Fixed in version: 4.6
  - [ ] GIF Walkthrough: ![XSS](https://github.com/maikamarquette/Cybersecurity-Week-7/blob/master/XXS.gif) 
  - [ ] Steps to recreate: 
    - Log onto wordpress as admin.
    - Go to a post.
    -Comment a XSS script in comment section.
    
  - [ ] Used source code: <IFRAME SRC="javascript:alert('XSS');"></IFRAME>
  
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
    
2. (Required) User Enumeration
  - [ ] Summary: 
    - Vulnerability types: User Enumeration
    - Tested in version: 4.2
    - Fixed in version: 4.7
  - [ ] GIF Walkthrough: ![User Enumeration](https://github.com/maikamarquette/Cybersecurity-Week-7/blob/master/User%20Enumeration.gif)
  - [ ] Steps to recreate: 
    - Go to the Wordpress login page.
    - Try a different username and password combination.
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
    
3. (Required) XSS exploit by uploading file
  - [ ] Summary: 
    - Vulnerability types: XSS (in file)
    - Tested in version: 4.2
    - Fixed in version: 4.9.1
  - [ ] GIF Walkthrough: ![](https://github.com/maikamarquette/Cybersecurity-Week-7/blob/master/XXS%20file.gif)
  - [ ] Steps to recreate: 
    - Log into wordpress.com as an admin.
    - Go to a new post.
    - Upload the .html file that you have created.
    - Publish the file and preview to exploit.
    
  - [ ] Used source code: <SCRIPT>alert('XSS')</SCRIPT> 
  
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [yyyy] [Maika Marquette]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
