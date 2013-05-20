zkstore
=======

## Introduction

In general, when we develop the website with zk, we divide webpage into header, body and footer with borderlayout. Sometimes we need the layout component which is easier to effectively use the space of a whole pagelayout. It should be columnlayout. Unlike the borderlayout, when the height of content is larger than the default height, then the vertical scrollbar should appear on the right side of the browser, not the content.

## Example Scenario

Suppose we want to create an online shopping website where user can read the news about latest items and can be easier to browse various kinds of items. Finally, we need the function which can show statistics of online shopper.

## Layout

Following figure shows the structure and how the columnlayout is placed on the screen. This webpage use columnlayout as body part.
[![](http://blog.zkoss.org/wp-content/uploads/2013/05/columnlayout0.png)](http://blog.zkoss.org/index.php/2013/05/14/how-to-use-columnlayout-to-layout-your-home-page/columnlayout0/)

## Live Demo

**New Page**

[![](http://blog.zkoss.org/wp-content/uploads/2013/05/columnlayout1-1024x569.png)](http://blog.zkoss.org/index.php/2013/05/14/how-to-use-columnlayout-to-layout-your-home-page/columnlayout1/)

**Shop Page**

[![](http://blog.zkoss.org/wp-content/uploads/2013/05/columnlayout2-1024x568.png)](http://blog.zkoss.org/index.php/2013/05/14/how-to-use-columnlayout-to-layout-your-home-page/columnlayout2/)

**Stats Page**

[![](http://blog.zkoss.org/wp-content/uploads/2013/05/columnlayout3-1024x579.png)](http://blog.zkoss.org/index.php/2013/05/14/how-to-use-columnlayout-to-layout-your-home-page/columnlayout3/)

## Layout Code

layout¡¦s code can be simplified as follows.

	<vlayout>
		<div sclass="header">...</div>
		<columnlayout sclass="body">
			<columnchildren sclass="sidebar">...</columnchildren>
			<columnchildren sclass="content">...</columnchildren>
		</columnlayout>
		<div sclass="footer">...</div>
	</vlayout>
	
know more about	[zkee](http://www.zkoss.org/product/zk)

Source: 
[https://github.com/huangnoah/zkstore](https://github.com/huangnoah/zkstore)

Reference:

[http://books.zkoss.org/wiki/Small_Talks/2008/June/Using_Columnlayout_Component](http://books.zkoss.org/wiki/Small_Talks/2008/June/Using_Columnlayout_Component)
[http://books.zkoss.org/wiki/ZK_Component_Reference/Layouts/Columnlayout](http://books.zkoss.org/wiki/ZK_Component_Reference/Layouts/Columnlayout)


## Copyright and License

<pre>
   Copyright 2013 Potix Corporation.

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
</pre>