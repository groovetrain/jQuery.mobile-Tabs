Creates simple jQuery.mobile tabs.

- Uses widget factory
- Follows normal jQuery mobile standards
- Implemented in a non-obtrusive way
- Programmed like a true jQuery novice :)

Usage
=====

First off, realize that this is a VERY rudimentary widget plugin, and that its use is fairly specific, meaning that I've only tested it one way, 
with the following **caveats**:

- Does not load any content via AJAX
- Does not load any different actual page parts, and depends on user doing some css in order to make some block-level items display as they would normally in jQuery.mobile
- Tab bar must be located in the header
- Content panels must be inside of the content area
- I hope to improve this sometime, or maybe the jQuery.mobile team will be able to use what I've got here to make something awesomer.

This being said, here's a sample of the usage:

`<div data-role="page" id="page-title">
  <div data-role="header">
    <h1><%= @page_title %></h1>
      <div data-role="tabs">
        <ul>
          <li><a href="#tab-1" class="">Tab 1</a></li>
          <li><a href="#tab-2" class="">Tab 2</a></li>
        </ul>
      </div>
  </div>
  
  <div data-role="content">
		<ul id="tab-1">
			<li>First thing</li>
			<li>Second Thing</li>
		</ul>
		
		<div id="tab-2">
			<h2>Here is the second tab</h2>
		</div>
  </div>
  
</div>`