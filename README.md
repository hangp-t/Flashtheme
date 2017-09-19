/*
Theme Name: Flash
Theme URI: https://themegrill.com/themes/flash
Author: ThemeGrill
Author URI: https://themegrill.com
Description: Flash is free responsive multipurpose WordPress theme – truly a versatile theme perfect for any type of website you want. Like never before, it provides multiple pre-built demos which can be imported in seconds using ThemeGrill Demo Importer Plugin. The theme fully integrates with Flash Toolkit and SiteOrigin’s Page Builder Plugin that makes theme more user-friendly and easy. Additionally, theme features multiple blog layouts, WooCommerce support, multiple header styles, multiple color options etc.
Version: 1.1.5
License: GNU General Public License v3 or later
License URI: http://www.gnu.org/licenses/gpl-3.0.html
Text Domain: flash
Tags: one-column, two-columns, left-sidebar, right-sidebar, grid-layout, custom-background, custom-colors, custom-menu, custom-logo, featured-images, footer-widgets, full-width-template, theme-options, threaded-comments, translation-ready, blog, e-commerce

Flash is based on Underscores http://underscores.me/, (C) 2012-2016 Automattic, Inc.
Underscores is distributed under the terms of the GNU GPL v2 or later.

Normalizing styles have been helped along thanks to the fine work of
Nicolas Gallagher and Jonathan Neal http://necolas.github.com/normalize.css/
*/


/*--------------------------------------------------------------
>>> TABLE OF CONTENTS:
----------------------------------------------------------------
# Normalize
# Typography
# Elements
# Forms
# Navigation
  ## Links
  ## Menus
# Accessibility
# Alignments
# Clearings
# Widgets
# Content
  ## Posts and pages
  ## Comments
# Infinite scroll
# Media
  ## Captions
  ## Galleries
  --------------------------------------------------------------*/


/*--------------------------------------------------------------
Normalize
--------------------------------------------------------------*/

html,
body,
div,
span,
applet,
object,
iframe,
h1,
h2,
h3,
h4,
h5,
h6,
p,
blockquote,
pre,
a,
abbr,
acronym,
address,
big,
cite,
code,
del,
dfn,
em,
font,
ins,
kbd,
q,
s,
samp,
small,
strike,
strong,
sub,
sup,
tt,
var,
dl,
dt,
dd,
ol,
ul,
li,
fieldset,
form,
label,
legend,
table,
caption,
tbody,
tfoot,
thead,
tr,
th,
td {
    border: 0;
    font-family: inherit;
    font-size: 100%;
    font-style: inherit;
    font-weight: inherit;
    margin: 0;
    outline: 0;
    padding: 0;
    vertical-align: baseline;
    word-break: break-word;
}

html {
    font-size: 62.5%;
    /* Corrects text resizing oddly in IE6/7 when body font-size is set using em units http://clagnut.com/blog/348/#c790 */
    overflow-y: scroll;
    /* Keeps page centered in all browsers regardless of content height */
    -webkit-text-size-adjust: 100%;
    /* Prevents iOS text size adjust after orientation change, without disabling user zoom */
    -ms-text-size-adjust: 100%;
    /* www.456bereastreet.com/archive/201012/controlling_text_size_in_safari_for_ios_without_disabling_user_zoom/ */
}

*,
*:before,
*:after {
    /* apply a natural box layout model to all elements; see http://www.paulirish.com/2012/box-sizing-border-box-ftw/ */
    /* Not needed for modern webkit but still used by Blackberry Browser 7.0; see http://caniuse.com/#search=box-sizing */
    /* Still needed for Firefox 28; see http://caniuse.com/#search=box-sizing */
    box-sizing: border-box;
}

body {
    background: #fff;
}

article,
aside,
details,
figcaption,
figure,
footer,
header,
main,
nav,
section {
    display: block;
}

ol,
ul {
    list-style: none;
}

table {
    border-collapse: separate;
    border-spacing: 0;
}

caption,
th,
td {
    font-weight: normal;
    text-align: left;
}

blockquote:before,
blockquote:after,
q:before,
q:after {
    content: "";
}

blockquote,
q {
    quotes: "" "";
}

a:focus {
    outline: 0;
}

a:hover,
a:active {
    outline: 0;
}

a img {
    border: 0;
    padding: 10px;
}
button.accordion {
    background-color: #427eb4;
    color: #ffffff;
    cursor: pointer;
    padding: 30px;
    border-radius: 3px;
    width: 100%;
    text-align: left;
    display: inline-block;
    border: none;
    outline: none;
    transition: 0.4s;
}
button.accordion.active, button.accordion:hover {
    background-color: #FFFFFF;
color:#333333;}

button.accordion:after {
    content: "\002B";
    color: #777;
    font-weight: bold;
    float: right;
    margin-left: 5px;
}

button.accordion.active:after {
    content: "\2212";
}
div.panel {
    padding: 0 18px;
    background-color: white;
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.2s ease-out;
}

#cf {
  position:relative;
  height:281px;
  width:450px;
  margin:0 auto;
}

#cf img {
  position:absolute;
  left:0;
  -webkit-transition: opacity 1s ease-in-out;
  -moz-transition: opacity 1s ease-in-out;
  -o-transition: opacity 1s ease-in-out;
  transition: opacity 1s ease-in-out;
}

#cf img.top:hover {
  opacity:0;
}

/*--------------------------------------------------------------
Typography
--------------------------------------------------------------*/

body,
button,
input,
select,
textarea {
    color: #333333;
    font-family: 'Montserrat', sans-serif;
    font-size: 14px;
    line-height: 1.5;
    font-weight: 400;
    text-rendering: optimizeLegibility;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}

b,
strong {
    font-weight: bold;
}

dfn,
cite,
em,
i {
    font-style: italic;
}

blockquote {
    margin: 0 15px;
    font-size: 20px;
    font-style: italic;
    font-family: 'Montserrat', sans-serif;
    font-weight: 300;
}

address {
    margin: 0 0 15px;
}

pre {
    background: #eee;
    font-family: 'Montserrat', sans-serif;
    font-size: 15px;
    font-size: 1.5rem;
    line-height: 1.6;
    margin-bottom: 1.6em;
    max-width: 100%;
    overflow: auto;
    padding: 1.6em;
}

code,
kbd,
tt,
var {
    font: 15px Monaco, Consolas, "Andale Mono", "DejaVu Sans Mono", monospace;
}

abbr,
acronym {
    border-bottom: 1px dotted #666;
    cursor: help;
}

mark,
ins {
    background: #fff9c0;
    text-decoration: none;
}

sup,
sub {
    font-size: 75%;
    height: 0;
    line-height: 0;
    position: relative;
    vertical-align: baseline;
}

sup {
    bottom: 1ex;
}

sub {
    top: .5ex;
}

small {
    font-size: 75%;
}

big {
    font-size: 125%;
}

h1 {
    font-size: 36px;
}

h2 {
    font-size: 30px;
}

h3 {
    font-size: 25px;
}

h4 {
    font-size: 20px;
}

h5 {
    font-size: 18px;
}

h6 {
    font-size: 16px;
}

h1,
h2,
h3,
h4,
h5,
h6 {
    font-weight: 700;
}


/*--------------------------------------------------------------
Elements
--------------------------------------------------------------*/

hr {
    background-color: #ccc;
    border: 0;
    height: 1px;
    margin-bottom: 15px;
}

ul,
ol {
    margin: 0 0 15px 20px;
}

ul {
    list-style: none;
}

ol {
    list-style: decimal;
}

li > ul,
li > ol {
    margin-bottom: 0;
    margin-left: 15px;
}

dt {
    font-weight: bold;
}

dd {
    margin: 0 15px 15px;
}

img {
    height: auto;
    /* Make sure images are scaled correctly. */
    max-width: 100%;
    /* Adhere to tg-container width. */
    vertical-align: middle;
}

figure {
    margin: 0;
}

table {
    margin: 0 0 15px;
    width: 100%;
    border-collapse: collapse;
}

th {
    font-weight: bold;
    border: 1px solid #CCC;
    padding: 5px 10px;
}

td {
    border: 1px solid #CCC;
    padding: 5px 10px;
}

p {
    margin: 0 0 30px;
}

/*--------------------------------------------------------------
Forms
--------------------------------------------------------------*/

button,
input,
select,
textarea {
    font-size: 100%;
    /* Corrects font size not being inherited in all browsers */
    margin: 0;
    /* Addresses margins set differently in IE6/7, F3/4, S5, Chrome */
    vertical-align: middle;
}

.navigation .nav-links a,
.bttn,
button,
input[type="button"],
input[type="reset"],
input[type="submit"] {
    background: #333333;
    color: #fff;
    cursor: pointer;
    /* Improves usability and consistency of cursor style between image-type 'input' and others */
    font-size: 14px;
    line-height: 13px;
    height: 33px;
    border: none;
    padding: 10px 15px;
    font-weight: 400;
    display: inline-block;
    position: relative;
    text-shadow: none;
    transition: background 0.5s ease;
    border-radius: 0;
    -webkit-appearance: none;
    -webkit-border-radius: 0px;
}

.navigation .nav-links a:hover,
.bttn:hover,
button,
input[type="button"]:hover,
input[type="reset"]:hover,
input[type="submit"]:hover {
    color: #ffffff;
}

input[type="checkbox"],
input[type="radio"] {
    padding: 0;
}

button::-moz-focus-inner,
input::-moz-focus-inner {
    /* Corrects inner padding and border displayed oddly in FF3/4 www.sitepen.com/blog/2008/05/14/the-devils-in-the-details-fixing-dojos-toolbar-buttons/ */
    border: 0;
    padding: 0;
}

input[type="text"],
input[type="email"],
input[type="url"],
input[type="password"],
input[type="search"] {
    color: #666;
    border: 1px solid #ccc;
    height: 36px;
    width: 100%;
    -webkit-appearance: none;
    border-radius: 0;
    -webkit-border-radius: 0px;
}

input[type="text"]:focus,
input[type="email"]:focus,
input[type="url"]:focus,
input[type="password"]:focus,
input[type="search"]:focus,
textarea:focus {
    border: 1px solid #AAA;
}

.searchform input[type="text"]:focus {
    border: none;
}

input[type="text"],
input[type="email"],
input[type="url"],
input[type="password"],
input[type="search"] {
    padding: 3px 6px;
}

textarea {
    overflow: auto;
    /* Removes default vertical scrollbar in IE6/7/8/9 */
    padding-left: 3px;
    vertical-align: top;
    /* Improves readability and alignment in all browsers */
    color: #666;
    border: 1px solid #ccc;
    height: 160px;
    max-width: 100%;
    width: 100%;
}


/*--------------------------------------------------------------
Links
--------------------------------------------------------------*/

a {
    color: #000;
    text-decoration: none;
    transition: all 0.3s ease-in-out;
    -webkit-transition: all 0.3s ease-in-out;
    -moz-transition: all 0.3s ease-in-out;
}

a:hover {
    color: #427eb4;
}


/*--------------------------------------------------------------
Clearings
--------------------------------------------------------------*/

.clearfix:before,
.clearfix:after,
.row:before,
.row:after,
.entry-content:before,
.entry-content:after,
.comment-content:before,
.comment-content:after,
.site-header:before,
.site-header:after,
.site-content:before,
.site-content:after,
.site-footer:before,
.site-footer:after,
.tg-container:after,
.tg-container:before {
    content: '';
    display: table;
}

.clearfix:after,
.row:after,
.entry-content:after,
.comment-content:after,
.site-header:after,
.site-content:after,
.site-footer:after,
.tg-container:after {
    clear: both;
}

.clear {
    clear: both;
}

.wp-caption,
.wp-caption-text,
.sticky,
.gallery-caption,
.bypostauthor {
    /*class required for wordpress*/
}

.alignright {
    text-align: right;
}

.alignleft {
    text-align: left;
}

.aligncenter {
    text-align: center;
}


/*--------------------------------------------------------------
grid
--------------------------------------------------------------*/

.tg-column-wrapper {
    clear: both;
    margin-left: -3%;
}

.tg-column-wrapper .tg-column-1,
.tg-column-wrapper .tg-column-2,
.tg-column-wrapper .tg-column-3,
.tg-column-wrapper .tg-column-4,
.tg-column-wrapper .tg-column-5 {
    float: left;
    margin-left: 3%;
}

.tg-column-wrapper .tg-column-1 {
    width: 100%;
}

.tg-column-wrapper .tg-column-2 {
    width: 47%;
}

.tg-column-wrapper .tg-column-3 {
    width: 30.33%;
}

.tg-column-wrapper .tg-column-4 {
    width: 22%;
}


/*--------------------------------------------------------------
Colors
--------------------------------------------------------------*/

.flash_inherit_color div,
.flash_inherit_color div.section-description,
.flash_inherit_color h1,
.flash_inherit_color h2,
.flash_inherit_color h3,
.flash_inherit_color h3.section-title,
.flash_inherit_color h4,
.flash_inherit_color h5,
.flash_inherit_color h6,
.flash_inherit_color p,
.flash_inherit_color span,
.flash_inherit_color div.service-content-wrap,
.flash_inherit_color .entry-summary {
    color: inherit !important;
}


/*--------------------------------------------------------------
 Galleries
--------------------------------------------------------------*/

.gallery {
    margin-bottom: 1.5em;
}

.gallery-item {
    display: inline-block;
    text-align: center;
    vertical-align: top;
    width: 100%;
}

.gallery-columns-2 .gallery-item {
    max-width: 50%;
}

.gallery-columns-3 .gallery-item {
    max-width: 33.33%;
}

.gallery-columns-4 .gallery-item {
    max-width: 25%;
}

.gallery-columns-5 .gallery-item {
    max-width: 20%;
}

.gallery-columns-6 .gallery-item {
    max-width: 16.66%;
}

.gallery-columns-7 .gallery-item {
    max-width: 14.28%;
}

.gallery-columns-8 .gallery-item {
    max-width: 12.5%;
}

.gallery-columns-9 .gallery-item {
    max-width: 11.11%;
}

.gallery-caption {
    display: block;
}


/*--------------------------------------------------------------
common
--------------------------------------------------------------*/

.tg-container {
    width: 1200px;
    margin: 0 auto;
}

.overlay {
    background-color: rgba(0, 0, 0, 0.5);
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
}

.screen-reader-text {
    clip: rect(1px, 1px, 1px, 1px);
    position: absolute !important;
    height: 1px;
    width: 1px;
    overflow: hidden;
}

#primary {
    float: left;
    width: 65.5%;
}

#secondary {
    float: right;
    width: 32.22%;
}

.page-template-full-width #primary,
.page-template-pagebuilder #primary {
    width: 100%;
}

#scroll-up {
    background-color: #30afb8;
    border-radius: 3px;
    bottom: 20px;
    color: #fff;
    display: none;
    padding: 10px 16px;
    position: fixed;
    opacity: 0.5;
    filter: alpha(opacity=50);
    /* For IE8 and earlier */
    right: 20px;
}

.post-navigation {
    margin-top: 30px;
    display: inline-block;
    width: 100%;
}

.post-navigation .nav-previous {
    float: left;
}

.post-navigation .nav-next {
    float: right;
}

.nav-next a .entry-title {
    float: left;
    margin-right: 3px;
}
.site{
    background-color: #fff;
}


/*--------------------------------------------------------------
}
Preloader CSS
--------------------------------------------------------------*/

#preloader {
    position: relative;
}

#preloader span {
    display: block;
    bottom: 0px;
    width: 9px;
    height: 5px;
    background: #21858c;
    position: absolute;
    -webkit-animation: preloader 1.5s infinite ease-in-out;
    -moz-animation: preloader 1.5s infinite ease-in-out;
    -ms-animation: preloader 1.5s infinite ease-in-out;
    -o-animation: preloader 1.5s infinite ease-in-out;
    animation: preloader 1.5s infinite ease-in-out;
}

#preloader span:nth-child(2) {
    left: 11px;
    -webkit-animation-delay: .2s;
    -moz-animation-delay: .2s;
    -ms-animation-delay: .2s;
    -o-animation-delay: .2s;
    animation-delay: .2s;
}

#preloader span:nth-child(3) {
    left: 22px;
    -webkit-animation-delay: .4s;
    -moz-animation-delay: .4s;
    -ms-animation-delay: .4s;
    -o-animation-delay: .4s;
    animation-delay: .4s;
}

#preloader span:nth-child(4) {
    left: 33px;
    -webkit-animation-delay: .6s;
    -moz-animation-delay: .6s;
    -ms-animation-delay: .6s;
    -o-animation-delay: .6s;
    animation-delay: .6s;
}

#preloader span:nth-child(5) {
    left: 44px;
    -webkit-animation-delay: .8s;
    -moz-animation-delay: .8s;
    -ms-animation-delay: .8s;
    -o-animation-delay: .8s;
    animation-delay: .8s;
}

@-webkit-keyframes preloader {
    0% {
        height: 5px;
        -webkit-transform: translateY(0px);
        background: #21858c;
    }
    25% {
        height: 30px;
        -webkit-transform: translateY(15px);
        background: #30aeb7;
    }
    50% {
        height: 5px;
        -webkit-transform: translateY(0px);
        background: #21858c;
    }
    100% {
        height: 5px;
        -webkit-transform: translateY(0px);
        background: #21858c;
    }
}

@-moz-keyframes preloader {
    0% {
        height: 5px;
        -moz-transform: translateY(0px);
        background: #21858c;
    }
    25% {
        height: 30px;
        -moz-transform: translateY(15px);
        background: #30aeb7;
    }
    50% {
        height: 5px;
        -moz-transform: translateY(0px);
        background: #21858c;
    }
    100% {
        height: 5px;
        -moz-transform: translateY(0px);
        background: #21858c;
    }
}

@-ms-keyframes preloader {
    0% {
        height: 5px;
        -ms-transform: translateY(0px);
        background: #21858c;
    }
    25% {
        height: 30px;
        -ms-transform: translateY(15px);
        background: #30aeb7;
    }
    50% {
        height: 5px;
        -ms-transform: translateY(0px);
        background: #21858c;
    }
    100% {
        height: 5px;
        -ms-transform: translateY(0px);
        background: #21858c;
    }
}

@keyframes preloader {
    0% {
        height: 5px;
        transform: translateY(0px);
        background: #21858c;
    }
    25% {
        height: 30px;
        transform: translateY(15px);
        background: #30aeb7;
    }
    50% {
        height: 5px;
        transform: translateY(0px);
        background: #21858c;
    }
    100% {
        height: 5px;
        transform: translateY(0px);
        background: #21858c;
    }
}

#spinners {
    position: absolute;
    top: 50%;
    left: 50%;
    -webkit-transform: translate(-50%, -50%);
    -moz-transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    -o-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
}

#preloader-background {
    background-color: #fff;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 9999;
}


/*--------------------------------------------------------------
Single page layout CSS
--------------------------------------------------------------*/

.left-sidebar #primary {
    float: right;
}

.left-sidebar #secondary {
    float: left;
}

.full-width #primary {
    float: none;
    width: 100%;
}

.full-width-center #primary {
    float: none;
    margin: 0 auto;
    width: 65.5%;
}


/*--------------------------------------------------------------
Header
--------------------------------------------------------------*/

.header-top {
    background-color: #f1f5f8;
}

.header-top .contact-info {
    line-height: 30px;
    float: left;
    margin: 0;
}

.header-top .tg-column-2 {
    width: auto;
}

.header-top .tg-column-2:last-child {
    float: right;
}

.header-top .contact-info li {
    float: left;
    font-size: 12px;
    color: #384554;
    margin-right: 30px;
    padding: 5px 0;
}

.header-top .contact-info li:last-child {
    margin-right: 0;
}

.header-top .social-menu {
    line-height: 30px;
    margin: 0;
    float: right;
}

.header-top .social-menu li {
    float: left;
    margin-left: 10px;
    font-size: 12px;
    padding: 5px 0;
}

.header-top .social-menu li:first-child {
    margin-left: 0;
}

.contact-info span {
    font-size: 16px;
    padding-right: 10px;
    color: #99a3b0;
}


/*-----------------Social menu-----------------*/

.social-menu li a {
    background-color: #fff;
    border-radius: 100%;
    font-size: 12px;
    font-family: fontawesome;
    text-align: center;
    display: inline-block;
    line-height: 30px;
    height: 30px;
    width: 30px;
    color: #99a3b0;
}

.transparent .social-menu li a {
    background-color: rgba(0, 0, 0, 0);
    border: none;
    color: #fff;
    height: auto;
    width: auto;
}

.social-menu li a[href*="facebook.com"]::before {
    content: "\f09a";
}

.social-menu li a[href*="linkedin.com"]::before {
    content: "\f0e1";
}

.social-menu li a[href*="twitter.com"]::before {
    content: "\f099";
}

.social-menu li a[href*="plus.google.com"]::before {
    content: "\f0d5";
}

.social-menu li a[href*="twitter.com"]:hover {
    color: #333333;
}

.social-menu li a[href*="plus.google.com"]:hover {
    color: #333333;
}

.social-menu li a[href*="linkedin.com"]:hover {
    color: #333333;
}

.social-menu li a[href*="facebook.com"]:hover {
    color: #333333;
}

.transparent .social-menu li a[href*="twitter.com"]:hover {
    color: #99a3b0;
}

.transparent .social-menu li a[href*="facebook.com"]:hover {
    color: #99a3b0;
}

.transparent .social-menu li a[href*="plus.google.com"]:hover {
    color: #99a3b0;
}

.transparent .social-menu li a[href*="linkedin.com"]:hover {
    color: #99a3b0;
}

.transparent .social-menu li a[href*="facebook.com"],
.transparent .social-menu li a[href*="linkedin.com"],
.transparent .social-menu li a[href*="twitter.com"],
.transparent .social-menu li a[href*="plus.google.com"] {
    color: #fff;
}

.transparent .is-sticky .social-menu li a[href*="facebook.com"],
.transparent .is-sticky .social-menu li a[href*="linkedin.com"],
.transparent .is-sticky .social-menu li a[href*="twitter.com"],
.transparent .is-sticky .social-menu li a[href*="plus.google.com"] {
    color: #333333;
}


/*-----------------Logo-----------------*/

.logo {
    float: left;
    padding: 0;
}

.logo .logo-image {
    float: left;
    padding: 20px 0;
}

.logo .logo-image a img {
    padding: 0;
}

.logo .logo-text {
    float: left;
    margin-left: 12px;
    padding: 11px 0;
}

.logo .logo-text p {
    margin: 0;
}

.logo-text .site-title {
    font-size: 22px;
    font-weight: 500;
    line-height: 24px;
}

.logo-text .site-title span {
    font-weight: 700;
}


/*-----------------Site Navigation-----------------*/

#site-navigation {
    float: right;
}

#site-navigation .menu-toggle {
    display: none;
}

#site-navigation ul {
    margin: 0;
}

#site-navigation ul li {
    float: left;
    padding: 23px 30px 23px 0;
    position: relative;
}

#site-navigation ul li a {
    font-size: 14px;
}

#site-navigation ul li:hover > a,
#site-navigation ul li.current-menu-item > a,
#site-navigation ul li.current_page_item > a {
    color: #30afb8;
}

#site-navigation ul li:last-child {
    padding-right: 0;
}

#site-navigation ul.sub-menu,
.menu ul li ul.children {
    background-color: #fff;
    min-width: 200px;
    padding: 0;
    position: absolute;
    box-shadow: 1px 1px 6px rgba(0, 0, 0, 0.2);
    right: 50%;
    top: 90%;
    -webkit-transform: translateX(50%);
    -moz-transform: translateX(50%);
    -ms-transform: translateX(50%);
    -o-transform: translateX(50%);
    transform: translateX(50%);
    opacity: 0;
    visibility: hidden;
    z-index: 9;
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
}

#site-navigation ul li ul li {
  padding: 10px;
  text-align: left;
  width: 100%;
}

#site-navigation ul.sub-menu li:hover {
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
}

#site-navigation ul.sub-menu li:hover a {
    color: #30afb8;
}

#site-navigation li:hover ul.sub-menu,
.menu ul li:hover > ul.children {
    opacity: 1;
    visibility: visible;
    top: 100%;
}

#site-navigation ul li a {
    color: #4c5867;
}

#site-navigation .sub-menu li.menu-item-has-children ul,
.menu ul li ul li ul.children {
    left: 50%;
    opacity: 0;
    visibility: hidden;
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
}

#site-navigation .sub-menu li.menu-item-has-children ul li:hover a {
    color: #30afb8;
}

#site-navigation .sub-menu li.menu-item-has-children ul li a {
    color: #4c5867;
}

#site-navigation ul li ul.sub-menu li.menu-item-has-children:hover ul,
.menu ul li ul li:hover ul.children {
    top: 0;
    opacity: 1;
    visibility: visible;
}

.sub-toggle {
    color: #333333;
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
}

#site-navigation ul li.menu-item-has-children:hover > .sub-toggle {
    color: #30afb8;
}

#site-navigation ul li ul.sub-menu li.menu-item-has-children .sub-toggle {
    position: absolute;
    top: 50%;
    right: 10px;
    -webkit-transform: translateY(-50%) rotate(-90deg);
    -moz-transform: translateY(-50%) rotate(-90deg);
    -ms-transform: translateY(-50%) rotate(-90deg);
    -o-transform: translateY(-50%) rotate(-90deg);
    transform: translateY(-50%) rotate(-90deg);
}

.transparent.header-sticky #masthead-sticky-wrapper.is-sticky #site-navigation ul li.current-flash-item a,
#site-navigation ul li.current-flash-item a {
    color: #30AFB8;
}

.header-bottom {
    background: #fff;
}


/*-----------------Header Search and Cart-----------------*/

.header-bottom .search-wrap {
    float: right;
    padding: 20px 0 20px 40px;
    position: relative;
}

.transparent.header-sticky .search-icon:hover,
.transparent .search-icon:hover,
.header-bottom .search-icon:hover {
    border-color: #30afb8;
    color: #30afb8;
}

.header-bottom .search-icon {
    cursor: pointer;
    color: #99a3b0;
    font-size: 14px;
    height: 30px;
    width: 30px;
    line-height: 30px;
    text-align: center;
    border: 1px solid #9ca6b2;
    border-radius: 100%;
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
}

.header-bottom .search-box {
    opacity: 0;
    visibility: hidden;
    position: absolute;
    width: 300px;
    top: 100%;
    right: -10px;
    background-color: #fff;
    box-shadow: 1px 1px 6px rgba(0, 0, 0, 0.2);
    padding: 20px;
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
}

.header-bottom .search-box.active {
    opacity: 1;
    visibility: visible;
    right: 0;
    z-index: 9;
}

.header-bottom .search-box .search-field {
    width: 80%;
    border-right: none;
    border-top: none;
    border-left: none;
    border-bottom: 1px solid #a1a1a1;
}

.header-bottom .searchform .btn {
    background-color: #30afb8;
}

.header-bottom .searchform .btn:hover {
    background-color: #2299a1;
}

.search-submit .fa {
    color: #fff;
}

.header-bottom .cart-wrap {
    float: right;
    padding: 20px 0 20px 30px;
    position: relative;
}

.header-bottom .flash-cart-views {
    font-size: 14px;
    height: 30px;
    width: 30px;
    line-height: 30px;
    text-align: center;
    border: 1px solid #9ca6b2;
    border-radius: 100%;
}

.header-bottom .flash-cart-views a {
    color: #99a3b0;
    position: relative;
}

.header-bottom .flash-cart-views a span {
    background-color: #30afb8;
    border-radius: 100%;
    font-size: 12px;
    left: 17px;
    height: 20px;
    width: 20px;
    line-height: 20px;
    text-align: center;
    position: absolute;
    top: -10px;
    color: #fff;
}

.header-bottom .widget_shopping_cart {
    opacity: 0;
    visibility: hidden;
    position: absolute;
    top: 100%;
    right: -10px;
    min-width: 250px;
    box-shadow: 1px 1px 6px rgba(0, 0, 0, 0.2);
    background-color: #fff;
    padding: 15px;
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
    z-index: 99;
}

.header-bottom .widget_shopping_cart ul {
    margin: 0;
}

.header-bottom .widget_shopping_cart ul li {
    text-align: center;
}

.header-bottom .cart-wrap:hover .widget_shopping_cart {
    opacity: 1;
    visibility: visible;
    right: 0;
    z-index: 9;
}

.boxed {
    width: 1200px;
    margin: 0 auto;
}

.boxed .site {
    background: #fff none repeat scroll 0 0;
    box-shadow: 0px 0px 12px 1px rgba(0, 0, 0, 0.3);
    margin: 30px 0;
    position: relative;
}

.boxed .tg-container {
    width: 100%;
    padding: 0 30px;
}

@media(max-width: 980px) {
    .boxed .tg-container {
        width: 98%;
    }
}

.transparent #masthead {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 999;
}

.transparent .header-top {
    background-color: transparent;
    border-bottom: 1px solid rgba(255, 255, 255, 0.3);
    color: #fff;
}

.transparent .contact-info span {
    color: #fff;
}

.transparent .contact-info li {
    color: #fff;
}

.transparent .header-bottom {
    border: none;
    background-color: transparent;
    border-bottom: 1px solid rgba(255, 255, 255, 0.3);
}

.transparent .logo-text,
.transparent .logo-text a {
    color: #fff;
}

.transparent.header-sticky #site-navigation ul li:hover > a {
    color: #30afb8;
}

.transparent #site-navigation .menu-toggle .fa,
.transparent #site-navigation ul li .sub-toggle {
    color: #fff;
}

.transparent #site-navigation ul.sub-menu li {
    padding: 0;
}

.transparent #site-navigation ul li a {
    color: #fff;
    display: inline-block;
}

.transparent #site-navigation ul li:hover .sub-toggle {
    color: #30afb8;
}

.transparent #site-navigation ul li:hover a {
    color: #30afb8;
    position: relative;
    visibility: none;
}

.transparent #site-navigation ul.sub-menu li a {
    color: #4c5867;
    padding: 10px 30px;
}

.transparent #site-navigation ul.sub-menu li a::before {
    display: none;
}

.transparent #site-navigation ul.sub-menu li:hover a,
.transparent #site-navigation ul.sub-menu li.menu-item-has-children ul li:hover a {
    color: #30afb8;
}

.transparent #site-navigation ul.sub-menu li.menu-item-has-children ul li a {
    color: #4c5867;
}

.transparent .cart-wrap .flash-cart-views {
    border-color: #fff;
}

.transparent .cart-wrap .flash-cart-views a {
    color: #fff;
}

.transparent .search-wrap .search-icon {
    color: #fff;
    border-color: #fff;
}

.right-logo-left-menu .logo {
    float: right;
}

.right-logo-left-menu #site-navigation {
    float: left;
}

.right-logo-left-menu #site-navigation ul li {
    padding: 20px 0 20px 30px;
}

.right-logo-left-menu #site-navigation ul lifirst-child {
    padding-left: 0;
}

.right-logo-left-menu .header-bottom .search-wrap {
    float: left;
    padding: 20px 30px 20px 0;
}

.right-logo-left-menu .header-bottom .cart-wrap {
    float: left;
    padding: 20px 30px 20px 0;
}

.center-logo-below-menu .logo {
    display: inline-block;
    float: none;
    width: 100%;
    text-align: center;
}

.center-logo-below-menu .logo .logo-text,
.center-logo-below-menu .logo .logo-image {
    float: none;
}

.center-logo-below-menu .logo .logo-image {
    padding: 20px 0 0 0;
    display: inline-block;
}

.center-logo-below-menu #site-navigation {
    float: left;
}

.header-sticky .is-sticky #masthead {
    z-index: 99 !important;
}
.header-sticky .is-sticky .header-bottom {
    background: #fff;
    box-shadow: 0 1px 1px rgba(0, 0, 0, 0.2);
}

.transparent.header-sticky #masthead-sticky-wrapper {
    left: 0;
    position: absolute;
    top: 0;
    width: 100%;
    z-index: 99;
}

.transparent.header-sticky #masthead {
    left: auto;
}

.transparent.header-sticky .header-top {
    display: none;
}

.transparent.header-sticky .header-bottom {
    background-color: transparent;
    border-bottom: 1px solid rgba(255, 255, 255, 0.3);
}

.transparent.header-sticky #site-navigation .menu-toggle .fa,
.transparent.header-sticky #site-navigation ul li a,
.transparent.header-sticky .flash-cart-views a {
    color: #fff;
}


.transparent.header-sticky #site-navigation ul.sub-menu li a {
    color: #333333;
}

.transparent.header-sticky #site-navigation ul.sub-menu li a:hover {
    color: #30afb8;
}

.transparent.header-sticky .flash-cart-views {
    border-color: #fff;
}


.transparent.header-sticky .search-icon {
    color: #fff;
    border-color: #fff;
}

.transparent.header-sticky .is-sticky #masthead {
    z-index: 99 !important;
}

.transparent.header-sticky .is-sticky .header-top {
    background: #f1f5f8;
    border: none;
    color: #333333;
    box-shadow: 0 1px 1px rgba(0, 0, 0, 0.2);
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
}

.transparent.header-sticky .is-sticky .header-top .contact-info li,
.transparent.header-sticky .is-sticky .header-top .contact-info li span,
.transparent.header-sticky .is-sticky .logo-text,
.transparent.header-sticky .is-sticky .logo-text a,
.transparent.header-sticky .is-sticky #site-navigation ul li a,
.transparent.header-sticky .is-sticky #site-navigation ul.sub-menu li a,
.transparent.header-sticky .is-sticky .flash-cart-views a {
    color: #333333;
}
.transparent.header-sticky .is-sticky .header-bottom {
    background: #fff;
    border: none;
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
}

.transparent.header-sticky .is-sticky .flash-cart-views {
    border-color: #333333;
}

.transparent.header-sticky .is-sticky .search-icon {
    color: #333333;
    border-color: #333333;
}

.transparent.header-sticky .custom-logo,
.transparent.header-sticky .is-sticky .transparent-logo,
.transparent-logo,
.transparent .custom-logo {
    display: none;
}

.transparent.header-sticky .is-sticky .custom-logo,
.transparent.header-sticky .transparent-logo,
.transparent .transparent-logo {
    display: block;
}

#wp-custom-header-video {
    display: block;
    min-height: 300px;
    min-height: 75vh;
    width: 100%;
}

.wp-custom-header {
    position: relative;
}

.wp-custom-header-video-button {
    position: absolute;
    bottom: 0;
    left: 0;
}

/*--------------------------------------------------------------
Slider
--------------------------------------------------------------*/

.tg-slider-widget .swiper-button-next {
    background-image: unset;
    right: 0;
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
    width: 50px;
    height: 50px;
    visibility: hidden;
    opacity: 0;
}

.tg-slider-widget .swiper-button-next::before {
    content: "\f105";
    font-family: fontawesome;
    font-size: 30px;
    color: #313b48;
    background: #fff;
    width: 50px;
    height: 50px;
    line-height: 50px;
    text-align: center;
    display: block;
}

.tg-slider-widget .swiper-button-prev {
    background-image: unset;
    left: 0;
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
    width: 50px;
    height: 50px;
    visibility: hidden;
    opacity: 0;
}

.tg-slider-widget .swiper-button-prev::before {
    content: "\f104";
    font-family: fontawesome;
    font-size: 30px;
    color: #313b48;
    background: #fff;
    width: 50px;
    height: 50px;
    line-height: 50px;
    text-align: center;
    display: block;
}

.tg-slider-widget:hover .swiper-button-next {
    right: 30px;
    visibility: visible;
    opacity: 1;
}

.tg-slider-widget:hover .swiper-button-prev {
    left: 30px;
    visibility: visible;
    opacity: 1;
}

.tg-slider-widget:hover .swiper-button-next.swiper-button-disabled {
    opacity: 0.36;
}

.tg-slider-widget:hover .swiper-button-prev.swiper-button-disabled {
    opacity: 0.36;
}

.tg-slider-widget .swiper-wrapper {
    position: relative;
}

.tg-slider-widget .swiper-slide {
    width: 100% !important;
}

.tg-slider-widget .slider-content {
    text-align: center;
    position: absolute;
    top: 50%;
    left: 50%;
    width: 100%;
    -webkit-transform: translate(-50%, -50%);
    -moz-transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    -o-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
}

.tg-slider-widget .caption-title {
    color: #313b48;
    font-size: 48px;
    font-weight: 800;
    line-height: 1.5;
    text-transform: uppercase;
}

.tg-slider-widget .caption-desc {
    font-size: 24px;
    line-height: 35px;
    margin: 10px 0 30px 0;
    text-transform: capitalize;
}

.tg-slider-widget .btn-wrapper {
    display: inline-block;
}

.tg-slider-widget .btn-wrapper a {
    border: 3px solid #313b48;
    display: inline-block;
    font-size: 20px;
    padding: 7px 26px;
}

.tg-slider-widget .btn-wrapper a:hover {
    background: #313b48;
    color: #fff;
    border-color: #313b48;
}

.tg-slider-widget.slider-content-left .slider-content {
    text-align: left;
    left: 0;
    -webkit-transform: translateY(-50%);
    -moz-transform: translateY(-50%);
    -ms-transform: translateY(-50%);
    -o-transform: translateY(-50%);
    transform: translateY(-50%);
}

.tg-slider-widget.slider-content-left .caption-title {
    width: 60%;
}

.tg-slider-widget.slider-content-left .caption-desc {
    font-size: 18px;
    line-height: 30px;
    width: 50%;
}

.tg-slider-widget.slider-light .slider-image .overlay {
    background-color: transparent;
}

.tg-slider-widget.slider-dark .slider-image .overlay {
    background-color: rgba(0, 0, 0, 0.5);
}

.tg-slider-widget.slider-dark .caption-title {
    color: #fff;
}

.tg-slider-widget.slider-dark .caption-desc {
    color: #fff;
}

.tg-slider-widget.slider-dark .btn-wrapper a {
    border-color: #fff;
    color: #fff;
}

.tg-slider-widget.slider-dark .btn-wrapper a:hover {
    border-color: #30afb8;
    background: #30afb8;
}
.full-screen.tg-slider-widget .slider-image img {
    height: 100%;
    max-width: none;
}
.slider-image {
  text-align: center;
}
/*--------------------------------------------------------------
Section Title
--------------------------------------------------------------*/

.section-title-wrapper {
    margin-bottom: 30px !important;
}

.section-title {
    color: #313b48;
    font-weight: 700;
    text-align: center;
    text-transform: uppercase;
    position: relative;
    margin-bottom: 20px;
}

.section-title:before,
.section-title:after {
    background: #e1e1e1 none repeat scroll 0 0;
    bottom: -5px;
    content: "";
    height: 1px;
    left: 50%;
    margin-left: -50px;
    position: absolute;
    width: 100px;
}

.section-title:after {
    background: #30afb8 none repeat scroll 0 0;
    bottom: -6px;
    height: 3px;
    margin-left: -15px;
    width: 30px;
}

.section-description {
    text-align: center;
    color: #777777;
}


/*--------------------------------------------------------------
About
--------------------------------------------------------------*/
.about-section .tg-column-wrapper{
    margin: 0;
}

.about-section .about-content-wrapper {
    display: table-cell;
    float: left;
    vertical-align: middle;
    padding-left: 3%;
}

.about-section .btn-wrapper {
    margin-top: 30px;
}

.about-section .btn-wrapper a {
    background-color: #30afb8;
    border-radius: 0;
    color: #fff;
    padding: 7px 35px;
}

.about-section .btn-wrapper a:hover {
    background-color: #2299a1;
}

.about-section .section-description {
    margin-top: 12px;
    text-align: left;
}
.about-content-wrapper .section-title {
  text-align: left;
}

.about-section .about-section-image {
    display: table-cell;
    float: right;
    margin-right: -5px;
    text-align: center;
    vertical-align: middle;
    padding-left: 3%;
}

.about-section .section-title::before, .about-section .section-title::after {
  left: 0;
  margin: 0;
  display: none;
}
.about-section .section-title::after {
    margin-left: 35px;
}


/*--------------------------------------------------------------
Service
--------------------------------------------------------------*/

.tg-service-widget .service-icon-wrap {
    background: #30afb8;
    color: #fff;
    display: block;
    float: left;
    font-size: 26px;
    height: 60px;
    line-height: 60px;
    margin-right: 20px;
    text-align: center;
    width: 60px;
    position: relative;
}

.tg-service-widget .service-icon-wrap:after {
    position: absolute;
    left: 50%;
    bottom: -9px;
    border-right: 10px solid transparent;
    border-left: 10px solid transparent;
    border-top: 10px solid #30afb8;
    content: "";
    -webkit-transform: translateX(-50%);
    -moz-transform: translateX(-50%);
    -ms-transform: translateX(-50%);
    -o-transform: translateX(-50%);
    transform: translateX(-50%);
}

.tg-service-widget .service-title-wrap {
    color: #313b48;
    font-size: 18px;
    font-weight: 700;
    line-height: 1.5;
    margin-top: 15px;
}

.tg-service-widget .service-title-wrap a:hover {
    color: #30afb8;
}

.tg-service-widget .service-content-wrap {
    margin: 10px 0;
    color: #777777;
}


/*-----------------tg-service-layout-2 -----------------*/

.tg-service-widget.tg-service-layout-2 .service-content-wrap {
    margin: 0 0 10px;
}

.tg-service-widget .service-more {
    font-weight: 600;
    font-size: 13px;
    color: #30afb8;
    display: inline-block;
    position: relative;
}
.tg-service-widget .service-more:hover {
  color: #1c9ba4;
}
.tg-service-widget .service-more:after {
    content: "\f178";
    font-family: FontAwesome;
    font-weight: 400;
    position: absolute;
    right: -22px;
    top: 0;
}

.tg-service-widget.tg-service-layout-2 {
    text-align: center;
}

.tg-service-widget.tg-service-layout-2 .service-icon-wrap {
    background: transparent none repeat scroll 0 0;
    border-radius: 50%;
    color: #000;
    display: block;
    float: none;
    font-size: 22px;
    height: 72px;
    line-height: 72px;
    margin: 0 auto;
    position: relative;
    text-align: center;
    width: 72px;
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    -ms-transition: all 0.5s ease;
    -o-transition: all 0.5s ease;
    transition: all 0.5s ease;
}

.tg-service-widget.tg-service-layout-2 .service-icon-wrap::after {
    display: none;
}

.tg-service-widget.tg-service-layout-2 .service-icon-wrap::before {
    border: 2px solid #000;
    border-radius: 100%;
    content: "";
    height: 82px;
    left: 50%;
    margin-left: -41px;
    margin-top: -41px;
    position: absolute;
    top: 50%;
    width: 82px;
}

.tg-service-widget.tg-service-layout-2 .service-icon-wrap:hover {
    background: #000 none repeat scroll 0 0;
    color: #fff;
}

.tg-service-widget.tg-service-layout-2 .service-title-wrap a {
    line-height: 24px;
}

.tg-service-widget.tg-service-layout-3 .service-title-wrap {
    line-height: 24px;
    margin-top: 20px;
}


/*-----------------tg-service-layout-3 -----------------*/

.tg-service-widget.tg-service-layout-3 .service-content-wrap {
    margin: 15px 0;
}

.tg-service-layout-2 .service-title-wrap {
    margin: 15px 0 5px;
}

.service-image-wrap img {
    width: 100%;
}


/*--------------------------------------------------------------
Team
--------------------------------------------------------------*/

.team-wrapper .team-content-wrapper {
    padding-top: 30px;
    position: relative;
    text-align: center;
}

.team-wrapper .team-title {
    font-size: 18px;
}

.team-wrapper .team-title a {
    color: #313b48;
}

.team-wrapper .team-title a:hover {
    color: #2299a1;
}

.team-wrapper .team-designation {
    position: relative;
}

.tg-team-widget img {
    width: 100%;
}

.team-wrapper .team-designation:after {
    position: absolute;
    left: 50%;
    bottom: -10px;
    width: 30px;
    height: 2px;
    background: #30afb8;
    content: "";
    -webkit-transform: translateX(-50%);
    -moz-transform: translateX(-50%);
    -ms-transform: translateX(-50%);
    -o-transform: translateX(-50%);
    transform: translateX(-50%);
}

.team-wrapper .team-content {
    color: #777777;
    margin: 30px 0 20px;
}

.team-wrapper .team-social {
    background: #fff none repeat scroll 0 0;
    left: 50%;
    margin-left: -45%;
    padding: 10px 0;
    position: absolute;
    top: -20px;
    width: 90%;
}

.team-wrapper .team-social a {
    font-size: 18px;
    margin: 0 8px;
}

.team-wrapper .team-social a:hover {
    color: #2299a1;
}


/*-----------------tg-team-layout-2 -----------------*/

.tg-team-widget.tg-team-layout-2 {
    position: relative;
}

.tg-team-widget.tg-team-layout-2::before {
    border-bottom: 50px solid transparent;
    border-right: 67px solid #fff;
    content: " ";
    position: absolute;
    right: 0;
    top: 0;
}

.tg-team-widget.tg-team-layout-2 .team-content-wrapper {
    text-align: left;
}

.tg-team-widget.tg-team-layout-2 .team-designation::after {
    left: 15px;
}

.tg-team-widget.tg-team-layout-2 .team-social {
    position: static;
    margin-left: 0;
    width: 100%;
    background: transparent;
    border-top: 1px solid #e7e7e7;
}


/*-----------------tg-team-layout-3 -----------------*/

.tg-team-widget.tg-team-layout-3::before {
    display: none;
}

.tg-team-widget.tg-team-layout-3 .team-img {
    position: relative;
}

.tg-team-widget.tg-team-layout-3 .team-img img {
    border-radius: 50%;
    width: 100%;
}

.tg-team-widget.tg-team-layout-3 .team-img .team-social {
    background: rgba(60, 180, 186, 0.8) none repeat scroll 0 0;
    border-radius: 50%;
    border-top: medium none;
    height: 100%;
    left: 0;
    padding: 0;
    position: absolute;
    top: 0;
    width: 100%;
    margin: 0;
    opacity: 0;
    visibility: hidden;
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
}

.tg-team-widget.tg-team-layout-3 .team-social-block {
    position: absolute;
    top: 50%;
    left: 0;
    width: 100%;
    text-align: center;
}

.tg-team-widget.tg-team-layout-3 .team-social-block a {
    font-size: 18px;
    margin: 0 8px;
    color: #fff;
}

.tg-team-widget.tg-team-layout-3 .team-content-wrapper {
    position: unset;
    padding-top: 30px;
    text-align: center;
}

.tg-team-widget.tg-team-layout-3 .team-designation::after {
    display: none;
}

.tg-team-widget.tg-team-layout-3 .team-content {
    display: none;
}

.tg-team-widget.tg-team-layout-3 .team-wrapper:hover .team-social {
    opacity: 1;
    visibility: visible;
}


/*--------------------------------------------------------------
Call To Action
--------------------------------------------------------------*/

.call-to-action-section {
    position: relative;
}

.call-to-action-section .section-title-wrapper .section-title {
    color: #fff;
    font-size: 32px;
}

.call-to-action-section .section-title::before,
.call-to-action-section .section-title::after {
    display: none;
}

.call-to-action-section .section-subtitle {
    color: #fff;
    font-size: 14px;
    line-height: 1.5;
    position: relative;
    text-align: center;
}

.call-to-action-section .btn-wrapper {
    text-align: center;
    margin-top: 30px;
}

.call-to-action-section .btn-wrapper a {
    border: 1px solid;
    border-radius: 50px;
    color: #fff;
background-color:#447c80;
    font-size: 22px;
    height: 50px;
    line-height: 50px;
    position: relative;
    margin-left: 30px;
    padding: 0 20px;
    display: inline-block;
}

.call-to-action-section .btn-wrapper a:first-child {
    margin-left: 0;
}

.call-to-action-section .btn-wrapper a:hover {
    background-color: #ffffff;
    border-color: #eeeeee;
}


/*----------------- call-to-action-section-layout-2 -----------------*/

.call-to-action-section .call-to-action-section-layout-2 {
    display: table;
    width: 100%;
}

.call-to-action-section .call-to-action-section-layout-2 .section-title-wrapper {
    display: table-cell;
    width: 75%;
    vertical-align: middle;
}

.call-to-action-section .call-to-action-section-layout-2 .section-title {
    margin-bottom: 0;
    text-align: left;
}

.call-to-action-section .call-to-action-section-layout-2 .section-subtitle {
    color: #fff;
    font-size: 14px;
    padding: 0 10px;
    position: relative;
    text-align: left;
}

.call-to-action-section .call-to-action-section-layout-2 .btn-wrapper {
    width: 25%;
    display: table-cell;
    vertical-align: middle;
    margin-top: 0;
}

.call-to-action-section .call-to-action-section-layout-2 .btn-wrapper a {
    display: block;
}

.call-to-action-section .call-to-action-section-layout-2 .btn-wrapper a:first-child {
    margin-left: 30px;
    margin-bottom: 15px;
}
/*--------------------------------------------------------------
Feature product
--------------------------------------------------------------*/

.feature-product-section .tg-feature-product-widget {
    position: relative;
    margin-bottom: 30px;
    overflow: hidden;
}

.feature-product-section .tg-feature-product-widget figure img {
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
}

.feature-product-section .featured-image-desc {
    visibility: hidden;
    opacity: 0;
    position: absolute;
    top: 50%;
    left: 50%;
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
    -webkit-transform: translate(-50%, -50%) scale(0);
    -moz-transform: translate(-50%, -50%) scale(0);
    -ms-transform: translate(-50%, -50%) scale(0);
    -o-transform: translate(-50%, -50%) scale(0);
    transform: translate(-50%, -50%) scale(0);
    width: 90%;
    height: 90%;
    background: rgba(49, 59, 73, 0.65);
}

.feature-product-section .tg-feature-product-widget .feature-inner-block {
    position: absolute;
    top: 50%;
    left: 0;
    width: 100%;
    padding: 5px;
    -webkit-transform: translateY(-50%);
    -moz-transform: translateY(-50%);
    -ms-transform: translateY(-50%);
    -o-transform: translateY(-50%);
    transform: translateY(-50%);
}

.feature-product-section .tg-feature-product-widget .feature-title-wrap {
    text-align: center;
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
}

.feature-product-section .tg-feature-product-widget .feature-title-wrap a {
    font-size: 16px;
    color: #fff;
    font-weight: 800;
}

.feature-product-section .tg-feature-product-widget .feature-desc-wrap {
    text-align: center;
    color: #f3f0f0;
    font-size: 12px;
}

.feature-product-section .tg-feature-product-widget .featured-image-desc::before {
    border-bottom: 50px solid transparent;
    border-right: 48px solid #30afb8;
    content: " ";
    position: absolute;
    right: 0;
    top: 0;
}

.feature-product-section .tg-feature-product-widget .featured-image-desc span {
    position: absolute;
    top: 4px;
    right: 7px;
}

.feature-product-section .tg-feature-product-widget .featured-image-desc span a {
    color: #fff;
}

.tg-feature-product-layout-1 .tg-feature-product-widget:hover .featured-image-desc,
.tg-feature-product-layout-2 .tg-feature-product-widget:hover .featured-image-desc {
    visibility: visible;
    opacity: 1;
    -webkit-transform: translate(-50%, -50%) scale(1);
    -moz-transform: translate(-50%, -50%) scale(1);
    -ms-transform: translate(-50%, -50%) scale(1);
    -o-transform: translate(-50%, -50%) scale(1);
    transform: translate(-50%, -50%) scale(1);
}


/*----------------- tg-feature-product-layout-2 -----------------*/

.feature-product-section .tg-feature-product-layout-2 .tg-container {
    width: 100%;
}

.feature-product-section .tg-feature-product-layout-2 .tg-column-wrapper,
.feature-product-section .tg-feature-product-layout-2 .tg-feature-product-widget {
    margin: 0;
}

.feature-product-section .tg-feature-product-layout-2 .tg-feature-product-widget.tg-column-3 {
    margin: 0;
    width: 33.33%;
}

.feature-product-section .tg-feature-product-layout-2 .tg-feature-product-widget.tg-column-4 {
    margin: 0;
    width: 25%;
}

.feature-product-section .tg-feature-product-layout-2 .tg-feature-product-widget img {
    width: 100%;
    max-width: auto;
}

.feature-product-section .tg-feature-product-layout-2 .featured-image-desc {
    width: 100%;
    height: 100%;
    padding: 5px;
    background: rgba(49, 175, 184, 0.8);
}

.feature-product-section .tg-feature-product-layout-2 .featured-image-desc::before {
    border-right: 48px solid #313b48;
}


/*----------------- tg-feature-product-layout-3 -----------------*/

.feature-product-section .tg-feature-product-layout-3 .featured-image-desc {
    visibility: visible;
    opacity: 1;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    -webkit-transform: scale(1);
    -moz-transform: scale(1);
    -ms-transform: scale(1);
    -o-transform: scale(1);
    transform: scale(1);
    background: transparent linear-gradient(to bottom, transparent, rgba(0, 0, 0, 0.5)) repeat scroll 0 0;
}

.feature-product-section .tg-feature-product-layout-3 .featured-image-desc::before,
.feature-product-section .tg-feature-product-layout-3 .featured-image-desc span,
.feature-product-section .tg-feature-product-layout-3 .feature-inner-block .feature-desc-wrap {
    display: none;
}

.feature-product-section .tg-feature-product-layout-3 .feature-inner-block {
    top: auto;
    -webkit-transform: translate(0);
    -moz-transform: translate(0);
    -ms-transform: translate(0);
    -o-transform: translate(0);
    transform: translate(0);
    bottom: 2%;
}

.feature-product-section .button-group {
    text-align: center;
    margin-bottom: 30px;
}

.feature-product-section .button-group button {
    background: transparent;
    color: #525a65;
}

.feature-product-section .button-group button:hover {
    color: #30afb8;
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
}

.feature-product-section .button-group button::before {
    background: #525a65 none repeat scroll 0 0;
    border-radius: 50%;
    content: " ";
    left: 0;
    margin-right: 50%;
    padding: 2px;
    position: absolute;
    top: 50%;
    -webkit-transform: translate(-50%, -50%);
    -moz-transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    -o-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
}

.tg-feature-product-filter-layout .button.is-checked:hover {
    color: #30afb8;
}

.tg-feature-product-layout-3 .tg-feature-product-widget:hover figure img {
    transform: scale(1.1);
    -webkit-transform: scale(1.1);
    -moz-transform: scale(1.1);
    -ms-transform: scale(1.1);
    -o-transform: scale(1.1);
}

.tg-feature-product-layout-3 .tg-feature-product-widget:hover .feature-title-wrap {
    margin-bottom: 3px;
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
}

/*--------------------------------------------------------------
Testimonial
--------------------------------------------------------------*/

.testimonial-container {
    padding: 0 0 50px;
}

.testimonial-container .testimonial-slide {
    text-align: left;
}

.testimonial-container .testimonial-content-wrapper {
    background: #fff;
    padding: 20px 30px;
    position: relative;
}

.testimonial-container .testimonial-content-wrapper::before {
    border-bottom: 34px solid transparent;
    border-left: 20px solid #fff;
    content: " ";
    left: 11%;
    position: absolute;
    top: 96%;
    -webkit-transform: rotate(12deg);
    -moz-transform: rotate(12deg);
    -ms-transform: rotate(12deg);
    -o-transform: rotate(12deg);
    transform: rotate(12deg);
    z-index: -9;
}

.testimonial-container .testimonial-icon {
    display: inline-block;
    vertical-align: top;
    color: #31afb8;
    font-size: 18px;
}

.testimonial-container .testimonial-content {
    width: 93%;
    display: inline-block;
    margin-left: 15px;
    color: #777777;
}

.testimonial-container .testimonial-client-detail {
    margin-top: 40px;
}

.testimonial-container .testimonial-img {
    display: inline-block;
    float: left;
}

.testimonial-container .client-detail-block {
    display: inline-block;
    margin-left: 20px;
}

.testimonial-container .testimonial-title {
    color: #313b48;
    font-size: 16px;
}

.testimonial-container .testimonial-degicnation {
    color: #666666;
    font-size: 14px;
    font-weight: 400;
}

.testimonial-container .swiper-pagination.testimonial-pager {
    bottom: 0;
}

.testimonial-container .swiper-pagination.testimonial-pager .swiper-pagination-bullet {
    width: 10px;
    height: 10px;
    background: #313b48;
    opacity: 1;
}

.testimonial-container .swiper-pagination.testimonial-pager .swiper-pagination-bullet:hover,
.testimonial-container .swiper-pagination.testimonial-pager .swiper-pagination-bullet.swiper-pagination-bullet-active {
    background: #2299a1;
}


/*--------------------------------------------------------------
Fun Facts
--------------------------------------------------------------*/

.fun-facts-section {
    text-align: center;
    color: #fff;
}

.fun-facts-icon-wrap {
    display: block;
    text-align: center;
    color: #30afb8;
    font-size: 64px;
    line-height: 1.5;
}

.fun-facts-section .counter-wrapper {
    font-size: 46px;
    font-weight: 700;
    line-height: 46px;
    display: block;
    margin-bottom: 15px;
}

.fun-facts-section .fun-facts-title-wrap {
    display: block;
    font-size: 16px;
    font-weight: 400;
    color: #fff;
}


/*----------------- tg-fun-facts-layout-2 -----------------*/

.tg-fun-facts-widget.tg-fun-facts-layout-2 .fun-facts-icon-wrap {
    background-color: rgba(255, 255, 255, 0.2);
    border: 5px solid rgba(255, 255, 255, 0.5);
    border-radius: 100%;
    color: #fff;
    display: inline-block;
    font-size: 36px;
    line-height: 120px;
    width: 120px;
    height: 120px;
}

.tg-fun-facts-widget.tg-fun-facts-layout-2 .fun-facts-title-wrap {
    line-height: 15px;
}

.tg-fun-facts-widget.tg-fun-facts-layout-2 .counter-wrapper {
    font-size: 46px;
    color: #30afb8;
    margin: 10px 0;
}


/*--------------------------------------------------------------
Blogs
--------------------------------------------------------------*/

.blog-section .tg-column-2 {
    margin: 0;
}

.blog-section .tg-blog-widget-layout-1 .tg-column-2 {
    width: 50%;
}

.blog-section .row:nth-child(odd) {
    float: left;
    width: 100%;
    background-color: #fcfcfc;
}

.blog-section .tg-blog-widget-layout-1 .row:nth-child(odd) .post-image {
    float: left;
    width: 50%;
    position: relative;
}

.blog-section .row:nth-child(odd) .post-image figure img {
    width: 100%;
}

.blog-section .row:nth-child(odd) .post-image::before {
    border-bottom: 15px solid transparent;
    border-right: 15px solid #fcfcfc;
    border-top: 15px solid transparent;
    content: " ";
    font-size: 22px;
    position: absolute;
    top: 50%;
    right: 0;
    -webkit-transform: translateY(-50%);
    -moz-transform: translateY(-50%);
    -ms-transform: translateY(-50%);
    -o-transform: translateY(-50%);
    transform: translateY(-50%);
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
}

.blog-section .tg-blog-widget-layout-1 .blog-content:hover .entry-title a {
    color: #fff;
}

.blog-section .row:nth-child(odd) .blog-content {
    float: left;
    padding: 15px 5px 15px 20px;
    width: 50%;
}

.blog-section .row:nth-child(odd) .post-readmore {
    display: none;
}

.blog-section .row:nth-child(odd) .entry-title {
    line-height: 24px;
}

.blog-section .row:nth-child(odd) .entry-title a {
    font-size: 18px;
    font-weight: 700;
    color: #313b48;
}

.blog-section .tg-blog-widget-layout-1 .tg-blog-widget:hover .blog-content .entry-title a {
    color: #fff;
}

.blog-section .row:nth-child(odd) .entry-title a:hover {
    color: #30afb8;
}

.blog-section .row:nth-child(odd) .entry-meta {
    margin: 8px 0;
    color: #919191;
}

.blog-section .row:nth-child(odd) .entry-meta .fa {
    padding-right: 5px;
}

.blog-section .row:nth-child(odd) .entry-meta a {
    font-size: 12px;
    color: #919191;
}

.blog-section .row:nth-child(odd) .entry-meta .entry-author {
    margin-left: 15px;
}

.blog-section .row:nth-child(odd) .entry-summary {
    font-size: 14px;
    color: #777777;
    font-weight: 400;
}

.blog-section .tg-blog-widget-layout-1 {
    margin: 0;
}

.tg-blog-widget-layout-1 .entry-summary {
    max-height: 167px;
    overflow: hidden;
}

.blog-section .row:nth-child(even) {
    float: left;
    width: 100%;
    background-color: #fcfcfc;
}

.blog-section .row:nth-child(even) .post-image {
    float: right;
    position: relative;
    width: 50%;
}

.blog-section .row:nth-child(even) .post-image figure img {
    width: 100%;
}

.tg-blog-widget-layout-1 .tg-blog-widget .entry-summary {
    margin: 0;
}

.blog-section .row:nth-child(even) .post-image::before {
    border-bottom: 15px solid transparent;
    border-left: 15px solid #fcfcfc;
    border-top: 15px solid transparent;
    content: " ";
    font-size: 22px;
    position: absolute;
    left: 0;
    top: 50%;
    -webkit-transform: translateY(-50%);
    -moz-transform: translateY(-50%);
    -ms-transform: translateY(-50%);
    -o-transform: translateY(-50%);
    transform: translateY(-50%);
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
}

.blog-section .row:nth-child(even) .blog-content {
    float: right;
    padding: 15px 5px 15px 20px;
    width: 50%;
}

.blog-section .row:nth-child(even) .post-readmore {
    display: none;
}

.blog-section .row:nth-child(even) .entry-title {
    line-height: 24px;
}

.blog-section .row:nth-child(even) .entry-title a {
    font-size: 18px;
    font-weight: 700;
    color: #313b48;
}

.blog-section .row:nth-child(even) .entry-title a:hover {
    color: #30afb8;
}

.blog-section .row:nth-child(even) .entry-meta {
    margin: 8px 0;
    color: #919191;
}

.blog-section .row:nth-child(even) .entry-meta .fa {
    margin-right: 5px;
}

.blog-section .row:nth-child(even) .entry-meta a {
    font-size: 12px;
    color: #919191;
}

.blog-section .row:nth-child(even) .entry-meta .entry-author {
    margin-left: 15px;
}

.blog-section .row:nth-child(even) .entry-summary {
    font-size: 14px;
    color: #777777;
    font-weight: 400;
}

.blog-section .tg-blog-widget {
    -webkit-transition: all 0.5s ease;
    -moz-transition: all 0.5s ease;
    transition: all 0.5s ease;
}

.blog-section .tg-blog-widget-layout-1 .tg-blog-widget:hover {
    background-color: #30afb8;
}

.blog-section .tg-blog-widget-layout-1 .tg-blog-widget:hover .entry-title a {
    color: #fff;
}

.blog-section .tg-blog-widget-layout-1 .tg-blog-widget:hover .entry-title a:hover {
    color: #313b48;
}

.blog-section .tg-blog-widget-layout-1 .tg-blog-widget:hover .entry-meta {
    color: #fff;
}

.blog-section .tg-blog-widget-layout-1 .tg-blog-widget:hover .entry-meta a {
    color: #fff;
}

.blog-section .tg-blog-widget-layout-1 .tg-blog-widget:hover .entry-summary {
    color: #fff;
}

.blog-section .row:nth-child(odd) .tg-blog-widget:hover .post-image::before {
    border-right: 15px solid #30afb8;
}

.blog-section .row:nth-child(even) .tg-blog-widget:hover .post-image::before {
    border-left: 15px solid #30afb8;
}

.blog-section .tg-blog-widget-layout-1 .entry-title a:hover,
.blog-section .tg-blog-widget-layout-1 .tg-blog-widget:hover .blog-content .entry-title a:hover{
    color: #fff;
}


/*----------------- tg-blog-widget-layout-2 -----------------*/

.blog-section .tg-blog-widget-layout-2 .post-image {
    position: relative;
    width: auto;
    float: none;
}

.blog-section .tg-blog-widget-layout-2 .post-image img {
    width: 100%;
}

.blog-section .tg-blog-widget-layout-2 .post-image .entry-date {
    background: #30afb8;
    left: 0;
    padding: 10px;
    position: absolute;
    text-align: center;
    top: 0;
}

.blog-section .tg-blog-widget-layout-2 .post-image .entry-date .fa {
    display: none;
}

.blog-section .tg-blog-widget-layout-2 .post-image .entry-date a {
    color: #fff;
    font-size: 12px;
}

.blog-section .tg-blog-widget-layout-2 .post-image::before {
    display: none;
}

.blog-section .tg-blog-widget-layout-2 .blog-content {
    float: none;
    padding: 0 10px;
    width: auto;
    text-align: left;
}

.blog-section .tg-blog-widget-layout-2 .entry-title a {
    font-size: 18px;
    line-height: 24px;
    display: block;
}

.tg-blog-widget-layout-2 .entry-title {
    margin-top: 15px;
}

.blog-section .tg-blog-widget-layout-2 .post-readmore {
    background: #30afb8;
    color: #fff;
    display: inline-block;
    font-size: 12px;
    padding: 6px 12px;
    margin: 20px 0;
}

.blog-section .tg-blog-widget-layout-2 .post-readmore:hover {
    background: #2299a1;
}

.blog-section .tg-blog-widget-layout-2 .read-more-container {
    background: #f6f6f6;
    display: inline-block;
    width: 100%;
    padding: 5px 10px;
    margin-top: 20px;
}

.blog-section .tg-blog-widget-layout-2 .read-more-container .entry-author {
    float: left;
    color: #8e8e8e;
}

.tg-blog-widget-layout-2 .read-more-container .entry-author a {
    color: #8e8e8e;
    font-size: 12px;
}

.blog-section .tg-blog-widget-layout-2 .read-more-container .entry-author .fa {
    margin-right: 5px;
}

.blog-section .tg-blog-widget-layout-2 .read-more-container .read-more {
    float: right;
}

.blog-section .tg-blog-widget-layout-2 .read-more-container .read-more a {
    font-size: 12px;
    color: #30afb8;
}

.blog-section .tg-blog-widget-layout-2:hover {
    background-color: #FCFCFC;
}
.blog-section .tg-blog-widget-layout-2:hover .entry-meta a {
    color: #919191;
}

.tg-blog-widget-layout-2 .blog-content p {
    margin: 0 0 10px;
}

.blog-section .tg-blog-widget-layout-2 .entry-title a:hover,
.blog-section .tg-blog-widget-layout-2 .tg-blog-widget:hover .blog-content .entry-title a:hover,
.blog-section .tg-blog-widget-layout-2 .read-more-container .read-more:hover a,
.tg-blog-widget-layout-2 .read-more-container .entry-author:hover a,
.tg-blog-widget-layout-2 .read-more-container .entry-author:hover {
    color: #239CA4;
}

/*--------------------------------------------------------------
Clients
--------------------------------------------------------------*/


/*--------------------------------------------------------------
Footer
--------------------------------------------------------------*/

#top-footer {
    background-color: #313b48;
    padding: 80px 0 30px;
}

#top-footer .footer-logo {
    display: inline-block;
    width: 100%;
    margin-bottom: 15px;
}

#top-footer .footer-logo .logo-image {
    float: left;
    padding: 5px;
}

#top-footer .footer-logo .site-title {
    font-size: 32px;
    color: #fff;
    font-weight: 700;
    float: left;
    line-height: 42px;
}

#top-footer .textwidget {
    font-size: 15px;
    color: #fff;
    line-height: 24px;
    font-weight: 400;
}

#top-footer .widget-title {
    font-size: 18px;
    border-left: 3px solid #30afb8;
    font-weight: 600;
    line-height: 24px;
    color: #fff;
    margin-bottom: 30px;
    padding-left: 20px;
}

#top-footer .widget-title::first-letter {
    color: #30afb8;
}

#top-footer .widget {
    margin-bottom: 30px;
}

#top-footer .widget ul {
    margin: 0;
}

#top-footer .widget ul li {
    position: relative;
    padding: 0 0 10px 20px;
    font-size: 12px;
}

#top-footer .widget ul li::after {
    color: #fff;
    content: "\f105";
    font-family: fontawesome;
    left: 0;
    position: absolute;
    top: 0;
}

#top-footer .widget ul li a {
    font-size: 14px;
    color: #fff;
}

#top-footer .widget ul li a:hover {
    color: #30afb8;
}

#top-footer .widget_tag_cloud .tagcloud a {
    border: 1px solid #fff;
    color: #fff;
    display: inline-block;
    margin: 6px 4px;
    padding: 0 5px;
}

#top-footer .widget_tag_cloud .tagcloud a:hover {
    background-color: #30afb8;
    border-color: #30afb8;
}

#bottom-footer {
    padding: 20px 0;
    background-color: #28313d;
}

#bottom-footer .copyright {
    float: left;
}

#bottom-footer .copyright-text {
    color: #fff;
    font-size: 12px;
}

#bottom-footer .copyright-text a {
    color: #bcbaba;
}

#bottom-footer .copyright-text a:hover {
    color: #30afb8;
}

#bottom-footer .footer-menu {
    float: right;
    margin: 0;
}

#bottom-footer .footer-menu ul li {
    float: left;
}

#bottom-footer .footer-menu ul li::after {
    content: "|";
    padding: 0 5px;
    color: #fff;
}

#bottom-footer .footer-menu ul li:last-child::after {
    display: none;
}

#bottom-footer .footer-menu ul li a {
    color: #fff;
    font-size: 12px;
}

#bottom-footer .footer-menu ul li a:hover {
    color: #30afb8;
}

.footer-menu li {
    float: left;
    padding: 0 0 0 15px;
}

.footer-menu li a {
    color: #fff;
    font-size: 12px;
}

.footer-menu li a:hover {
    color: #30afb8;
}


/*--------------------------------------------------------------
Archive
--------------------------------------------------------------*/

.post {
    margin-bottom: 40px;
    display: inline-block;
}

.post .entry-thumbnail {
    float: left;
    margin-right: 30px;
    width: 33.7%;
}

.entry-content-block {
    overflow: hidden;
}

.entry-meta .entry-date a .updated:not(.published) {
    display: none;
}

.entry-content-block #primary .entry-title {
    font-size: 20px;
    line-height: 24px;
}

.entry-content,
.entry-summary {
    margin-top: 12px;
    color: #606060;
}

#primary .entry-footer span {
    font-size: 14px;
    margin-right: 15px;
}

#primary .entry-footer span .fa {
    margin-right: 5px;
}

#primary .entry-footer span a {
    font-size: 12px;
}

.navigation.posts-navigation {
    margin: 20px 0;
}

.entry-meta {
    font-size: 12px;
    margin-top: 12px;
}

.entry-meta .fa {
    padding-right: 5px;
}

.entry-meta a, .entry-footer a {
    font-size: 12px;
    color: #8e8e8e;
}

.entry-meta span{
    margin-right: 15px;
}

.entry-meta .entry-author:hover{
    color: #30AFB8;
}

#secondary {
    float: right;
    width: 32.22%;
}

#secondary .widget-title {
    font-size: 14px;
    position: relative;
    margin-bottom: 30px;
}

#secondary .widget-title::before,
#secondary .widget-title::after {
    background: #e1e1e1 none repeat scroll 0 0;
    bottom: -10px;
    content: " ";
    height: 1px;
    left: 0;
    margin-left: 0;
    position: absolute;
    width: 100%;
}

#secondary .widget-title:after {
    background: #30afb8;
    bottom: -11px;
    height: 3px;
    margin-left: 0;
    width: 30px;
}

#secondary .searchform input {
    border: none;
    border-bottom: 1px solid #666;
    width: 70%;
}

#secondary .searchform .btn:hover {
    background: #30afb8 none repeat scroll 0 0;
}

#secondary .widget {
    margin-bottom: 30px;
}

#secondary .widget ul {
    margin: 0;
}

#secondary .widget ul li {
    position: relative;
    padding: 0 0 10px 20px;
    font-size: 12px;
}

#secondary .widget ul li::after {
    color: #000;
    content: "\f105";
    font-family: fontawesome;
    left: 0;
    position: absolute;
    top: 0;
}

#secondary .widget ul li a {
    font-size: 12px;
}

#secondary .widget ul li a:hover {
    color: #30afb8;
}

.widget_post_list .post-link-block  {
    margin-bottom: 20px;
    display: inline-block;
}

.widget_post_list .entry-thumbnail {
    float: left;
    margin-right: 30px;
    width: 20%;
}

.widget_post_list .entry-content-block {
    overflow: hidden;
}

.widget_post_list .entry-content-block .entry-title {
    line-height: 13px;
    margin-bottom: 18px;
}

.widget_post_list .entry-content-block .entry-title a {
    font-size: 12px;
}

.widget_post_list .entry-content-block .entry-meta a {
    color: #8e8e8e;
    font-size: 12px;
}

.widget_post_list .entry-meta .entry-author {
    margin-left: 15px;
}

.blog  .entry-thumbnail {
    float: left;
    width: 33.7%;
}

.blog .entry-content-block{
    width: 60%;
}

#primary .post .entry-content-block .entry-content {
    border: none;
}

.full-width-archive #primary .post{
    margin-bottom: 0;
    width: 100%;
}

.full-width-archive #primary .post .entry-thumbnail{
    width: 100%;
    float: none;
    margin-right: 0;
}

.full-width-archive #primary .post .entry-thumbnail img {
    width: 100%;
}

.full-width-archive #primary .post .entry-content-block {
    overflow: unset;
    width: 94%;
    position: relative;
    top: -45px;
    padding: 20px 20px 0 20px;
    margin: 0 auto;
    background: #fff;
}

.grid-view #primary .post {
    display: inline-block;
    margin-bottom: 30px;
    margin-right: 1%;
    vertical-align: top;
    width: 48%;
}

.grid-view #primary .post .entry-thumbnail {
    width: 100%;
}

.grid-view #primary .post .entry-content-block {
    position: unset;
    width: 100%;
}
.entry-content-block .entry-title {
    font-size: 18px;
}
.grid-view .entry-header{
    margin-top: 10px;
}
/*--------------------------------------------------------------
Bread Crumb
--------------------------------------------------------------*/

.breadcrumb-trail.breadcrumbs {
    background: #fafafa none repeat scroll 0 0;
    margin-bottom: 30px;
}

.breadcrumb-trail.breadcrumbs .trail-title {
    float: left;
    font-weight: 400;
    font-size: 25px;
    padding: 6px 0;
}

.breadcrumb-trail.breadcrumbs .trail-items {
    float: right;
    margin: 0;
    padding: 14px 0;
}

.breadcrumb-trail.breadcrumbs .trail-items li {
    float: left;
}

.breadcrumb-trail.breadcrumbs .trail-items li:first-child span::before {
    display: none;
}

.breadcrumb-trail.breadcrumbs::before {
    clear: both;
    content: "";
    display: block;
}

.breadcrumb-trail.breadcrumbs .trail-items li span {
    font-size: 12px;
    color: #a1a1a1;
    position: relative;
    line-height: 18px;
    padding: 0 14px;
}
.breadcrumb-trail.breadcrumbs .trail-items li span a {
    color: #a1a1a1;
}

.breadcrumb-trail.breadcrumbs .trail-items li span::before {
    color: #a1a1a1;
    content: "\f105";
    font-family: fontawesome;
    left: 0;
    position: absolute;
    top: 0;
}
.page-template-pagebuilder .breadcrumb-trail.breadcrumbs {
  margin: 0;
}

/*--------------------------------------------------------------
Post Page
--------------------------------------------------------------*/
.post {
    width: 100%;
}

.single .entry-content-block .entry-meta {
    margin-top: 0;
    margin-bottom: 20px;
}

.single .entry-content-block .entry-header {
    margin: 20px 0 5px;
}
.single .entry-thumbnail {
    margin-top: 20px;
    width: 100%;
}
.single .entry-thumbnail img {
    padding: 0;
}
.single .entry-content-block {
    width: 100%;
}
.single .entry-content-block .entry-title {
    font-size: 20px;
}
.single .entry-content-block .entry-meta .fa {
    padding-right: 5px;
}
.single .entry-content-block .entry-meta a {
    font-size: 12px;
}
.post .entry-content-block .entry-meta a:hover,
.post .entry-content-block .entry-meta span:hover{
    color: #30afb8;
}
.single .entry-content-block .entry-content {
    border-bottom: 1px solid #c5c5c5;
}
.single .entry-content-block .entry-footer span {
    color: #8e8e8e;
    font-size: 14px;
    margin-right: 15px;
}
.single .entry-content-block .entry-footer span .fa {
    margin-right: 5px;
}
.single .entry-content-block .entry-footer span a {
    color: #8e8e8e;
    font-size: 12px;
}
.post .entry-content-block .entry-footer span a:hover{
    color: #30AFB8;
}
.author-description {
    border-bottom: 1px solid #c5c5c5;
    display: inline-block;
    padding: 0 0 30px;
}
.author-description .author-img {
    display: inline-block;
    width: 75px;
    float: left;
}
.author-description .author-description-block {
    width: calc(100% - 100px);
    float: right;
    display: inline-block;
}
.author-description .author-description-block .author-title {
    color: #313b48;
    font-weight: 700;
}
.author-description .author-description-block .author-summary {
    font-size: 12px;
}
.default-wp-page {
    margin: 0;
    padding: 30px 0;
    display: inline-block;
    border-bottom: 1px solid #c5c5c5;
}
.default-wp-page .previous {
    float: left;
    width: 46%;
}
.default-wp-page .previous a {
    display: inline-block;
}
.default-wp-page .previous a span {
    float: left;
}
.default-wp-page .previous a span:first-child {
    font-size: 30px;
    padding: 8px 0;
}
.default-wp-page .previous a span img {
    padding: 0 10px;
}
.default-wp-page .previous a .entry-title {
    display: inline-block;
    width: 60%;
    padding: 8px 0;
}
.default-wp-page .navigation-divider {
    display: inline-block;
    padding: 20px;
}
.default-wp-page .next {
    float: right;
    width: 46%;
}
.default-wp-page .next a {
    display: inline-block;
}
.default-wp-page .next a span {
    float: right;
}
.default-wp-page .next a span:first-child {
    font-size: 30px;
    padding: 8px 0;
}
.default-wp-page .next a span img {
    padding: 0 10px;
}
.default-wp-page .next a .entry-title {
    display: inline-block;
    width: 60%;
    padding: 8px 0;
    text-align: right;
}


/*--------------------------------------------------------------
404 page
--------------------------------------------------------------*/

.not-found .icon-404 .fa {
    font-size: 300px;
}

#primary .content-404 {
    padding: 60px 0;
}

#primary .not-found .page-header .page-title {
    font-size: 24px;
    line-height: 30px;
}

#primary .not-found .page-content {
    margin: 30px 0;
}

#primary .searchform input {
    border: none;
    border-bottom: 1px solid #666;
    width: 70%;
}

#primary .searchform .btn:hover {
    background: #30afb8 none repeat scroll 0 0;
}

.search .hentry {
    border-bottom: 1px solid #e1e1e1;
    margin-top: 20px;
}


/*--------------------------------------------------------------
Comments
--------------------------------------------------------------*/

#comments {
    padding: 30px 0;
}

#comments .comments-title {
    font-size: 25px;
    line-height: 30px;
}

#comments .comment-list {
    margin: 0;
}

#comments .comment-list article.comment-body .comment-author {
    float: left;
    max-width: 100px;
}

#comments .comment-list article.comment-body .comment-author .says {
    display: none;
}

#comments .comment-list article.comment-body .comment-author img {
    margin-right: 30px;
    display: block;
    margin-bottom: 20px;
}

#comments .comment-list article.comment-body .comment-metadata {
    padding: 6px 0;
}

#comments .comment-list article.comment-body .comment-metadata a {
    color: #8e8e8e;
    font-size: 12px;
}

#comments .comment-list article.comment-body .comment-metadata .entry-author {
    margin-left: 15px;
}

#comments .comment-list article.comment-body .comment-content {
    overflow: hidden;
    font-weight: 500;
}

#comments .comment-list article.comment-body .comment-content p {
    margin: 0;
}

#comments .comment-list article.comment-body .reply {
    margin-left: 100px;
    padding-top: 6px;
}

#comments .comment-list article.comment-body .reply a {
    color: #8e8e8e;
    font-size: 12px;
    position: relative;
}

#comments .comment-list article.comment-body .reply a::before {
    position: absolute;
    top: 50%;
    left: 100%;
    content: " ";
    width: 30px;
    border: 1px solid #c5c5c5;
    -webkit-transform: translateY(-50%);
    -moz-transform: translateY(-50%);
    -ms-transform: translateY(-50%);
    -o-transform: translateY(-50%);
    transform: translateY(-50%);
    margin-left: 10px;
}

#comments .comment-list .comment {
    border-bottom: 1px solid #c1c1c1;
    padding: 30px 0;
}

#comments .comment-list .comment ul.children {
    margin-left: 100px;
}

#comments .comment-list .comment ul.children .comment {
    padding: 0;
    border-bottom: none;
}

#comments .comment-list .comment ul.children .comment article.comment-body {
    border-bottom: 1px solid #c1c1c1;
    padding: 20px 0;
}

#comments .comment-list .comment ul.children .comment article.comment-body:last-child {
    border: none;
}

#respond {
    padding-bottom: 10px;
}

#respond #commentform .comment-form-comment #comment {
    background: #f9f9f9 none repeat scroll 0 0;
    resize: none;
}

#respond #commentform p {
    padding-bottom: 20px;
}

#respond #commentform p label {
    font-weight: 500;
}

#respond #commentform p input {
    background: #f9f9f9 none repeat scroll 0 0;
}

#respond #commentform .form-submit input {
    background: #30afb8;
    height: 45px;
    line-height: 30px;
}
#respond #commentform .form-submit input:hover {
    background-color: #1c9ba4;
}

/*--------------------------------------------------------------
WooCommerce
--------------------------------------------------------------*/

.woocommerce ul.products li.product a img,
.woocommerce div.product div.images img {
    padding: 0;
}

.woocommerce span.onsale,
.woocommerce ul.products li.product .onsale {
    background-color: #30afb8;
    padding: 0;
    height: 50px;
    width: 50px;
    line-height: 50px;
}

#add_payment_method table.cart img, .woocommerce-cart table.cart img, .woocommerce-checkout table.cart img{
    width: auto;
}
.woocommerce ul.products li.product .button,
.woocommerce #respond input#submit.alt,
.woocommerce a.button.alt,
.woocommerce button.button.alt,
.woocommerce input.button.alt {
    background-color: #30afb8;
    color: #fff;
}

.woocommerce ul.products li.product .button:hover,
.woocommerce #respond input#submit.alt:hover,
.woocommerce a.button.alt:hover,
.woocommerce button.button.alt:hover,
.woocommerce input.button.alt:hover {
    background-color: #2299a1;
}

.added_to_cart.wc-forward {
    background-color: #30afb8;
    border-radius: 3px;
    font-size: 14px;
    line-height: 18px;
    color: #fff;
    padding: 4px 17px;
    margin-top: 5px;
}

.added_to_cart.wc-forward:hover {
    background-color: #2299a1;
}

.added_to_cart.wc-forward::after {
    content: "\f23d";
    color: #fff;
    font-family: fontawesome;
    padding-left: 8px;
}

.woocommerce-Price-amount.amount {
    color: #30afb8;
}

.woocommerce .star-rating span {
    color: #FFAE65;
}

.widget_shopping_cart .buttons {
    text-align: center;
}

.woocommerce .widget_shopping_cart .total,
.woocommerce.widget_shopping_cart .total {
    padding: 5px 0;
    text-align: center;
}

.flash-cart-views .woocommerce ul.cart_list li img,
.woocommerce ul.product_list_widget li img {
    width: 70px;
}

.woocommerce ul.products li.product .price del {
    margin-right: 5px;
    display: inline-block;
}

.woocommerce nav.woocommerce-pagination {
    text-align: left;
}

.woocommerce .woocommerce-breadcrumb {
    float: right;
    margin: 0;
    padding: 14px 0;
}

.woocommerce .woocommerce-breadcrumb span{
    font-size: 12px;
    color: #a1a1a1;
    position: relative;
    line-height: 18px;
    padding: 0 14px;
}

.woocommerce .woocommerce-breadcrumb span::before {
    color: #a1a1a1;
    content: "\f105";
    font-family: fontawesome;
    left: 0;
    position: absolute;
    top: 0;
}

.woocommerce .woocommerce-breadcrumb span:first-of-type::before{
	content: none;
}
