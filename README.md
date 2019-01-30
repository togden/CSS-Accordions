# CSS-Accordions
A simple and elegant solution for accordion elements using only HTML and CSS. Create collapsible bulleted lists without JavaScript.


<!DOCTYPE html>
<html>

    <head>
        <meta charset="utf-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <title>Messin' With Accordions</title>
        <meta name="description" content="An interactive getting started guide for Brackets.">
        <link rel="stylesheet" href="main.css">
    </head>
    <body>

        <h1>CSS + HTML only Accordion Element</h1>
        <ul>
            <li>
                <p>Hey, here's some un-hidden text to explain how this all works! Kinda cool, huh? This is the first element in our unordered list.</p>

                <ul>
                    <li>
                        <p>Here's a nested bullet point. Woo!</p>
                    </li>
                    <li>
                        <p>And Another!</p>
                    </li>
                </ul>
            </li>
            <li>
                <p>Here's another bullet point that is always visible.</p>
            </li>
            <li>
                <input type="checkbox" checked>            
                <p>This page was written in HTML and CSS. The CSS was compiled from SASS. I used Normalize as my CSS reset and -prefix-free to save myself some headaches. I haven't quite gotten the hang of Slim for compiling into HTML, but someday I'll use it since its syntax compliments that of SASS. Regardless, this could all be done in plain HTML and CSS.</p>
                <p>Here's a second paragraph disguised as a bulleted list, also hidden by default. This is only visible after expanding the list using the show more/less link.</p>

                <span class="expand-icon"></span><label class="expand-label"></label>
            </li>
        </ul>
        <ul>
            <li>
                <p>Hey, here's some un-hidden text to explain how this all works! Kinda cool, huh?</p>
            </li>
            <li>

                <input type="checkbox" checked>

                <p>Using the sibling and checked selectors, we can determine the styling of sibling elements based on the checked state of the checkbox input element. One use, as demonstrated here, is an entirely CSS and HTML accordion element. Media queries are used to make the element responsive to different screen sizes.</p>

                <span class="expand-icon"></span><label class="expand-label"></label>

            </li>
        </ul>
        <ul>
            <li>
                <p>Hey, here's some un-hidden text to explain how this all works! Kinda cool, huh?</p>
            </li>
            <li>
                <input type="checkbox" checked>

                <p>By making the open state default for when :checked isn't detected, we can make this system accessable for browsers that don't recognize :checked. The fallback is simply an open accordion. The accordion can be manipulated with Javascript (if needed) by changing the "checked" property of the input element.</p>
                <span class="expand-icon"></span><label class="expand-label" for="accordion-toggle"></label>

            </li>

        </ul>
    </body>
</html>
