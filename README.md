# Learning CSS

## Box Model
CSS is all boxes.
Boxes behave differently depending on their display value
You can control this by using extrinsic sizing, or, you can continue to let the browser make decisions for you based on the content size, using intrinsic sizing.
When content is too big for the box it is in, we call this overflow. You can manage how an element handles overflow content, using the overflow property. Overflow:auto or overflow:scroll will screate space in the padding.
The four main areas of the box model: content box, padding box, border box and margin box.
Margin box holds outline and box-shadow. They don't effect what's inside since these are painted on top. 
Box-sizing: content-box will size the content box sans padding and border. Do box-sizing: border-box if you'd like otherwise. 

## The Cascade
Understanding the cascade algorithm helps you understand how the browser resolves conflicts like this. The cascade algorithm is split into 4 distinct stages.
* Position and order of appearance: the order of which your CSS rules appear
An inline style attribute with CSS declared in it will override all other CSS, regardless of its position, unless a declaration has !important defined.
* Specificity: an algorithm which determines which CSS selector has the strongest match
Least specific to most tag < class < id
* Origin: the order of when CSS appears and where it comes from, whether that is a browser style, CSS from a browser extension, or your authored CSS
* Importance: some CSS rules are weighted more heavily than others, especially with the !important rule type