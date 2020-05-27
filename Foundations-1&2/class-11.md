## Chapter 16: “Images” (pp.406-427)
* for images, use class= , not id=
* you can put as many class names in an image tag as you'd like, for example an align and size indicator like below:
    * < img src="picture link" alt="name of picture" class="align-left" medium />
    * alt, other than being an accessibility tool for others, can be a tracking tool for you; easier to search and find the image you're wanting to manipulate
* quick css cheat sheet/reference points for image control:
    * SIZE
        * img.large {
            width: 500px;
            height: 500px
        }
        * img.medium {
            width: 250px;
            height: 250px;
        }
        * img.small {
            width: 100px;
            height: 100px;
        }
    * ALIGN
        * img.align.left {
            float: left;
            margin-right: 10px; (puts 10px margin on right)
        }
        * imag.align.right{
            float: right;
            margin-left: 10px; (puts 10px margin on left)
        }
        * img.align.center {
            display: block;
            margin: 0px auto; (0px margin for left and right) 
        }
    * background images:
        * body {
            background-image: url("picture link");
        }
        * p {
            background-image: url (" ");
        }
    * background repeat and attachment:
        * body {
            background-image: url (" ");
            background-repeat: repeat-x; (the image is repeated horizontally only)
            background-repeat: repeat-y; (the image is repeated vertically only);
        }
        * body {
            background-image: url(" ");
            background-repeat: no-repeat;
            background-attachment: fixed; (fixes image in the same position on the page )
            backgrounf-attachment: scroll; (image moves with up and down scroll)
        }
    * background position
        * when an image is not being repeated, you can use the background-position property to specify where in the browser window the background image should be placed
            * left..., center..., right...
                * ...top
                * ...center
                * ...bottom
            * example:
                * body {
                    background-image: url (" ");
                    background-repeat: no repeat;
                    background-position: center top;
                }
        * you can also use a pair of pixels or percentages that represent the distance from the top left corner of the browser or container 
            * the top left corner is equal to 0% 0%
* background shorthand can be done inside the div of the html but must follow the order of :
    1. background-color
    2. background-image
    3. background-repeat
    4. background-attachment
    5. backgroun-position
    * they must be specified in this order, but you can skill a value if you don't want to specify it 
        * example:
            div {
                background:
                    url (image)
                    no-repeat
                    etc. etc.
            }
* image rollover and sprites: pg 417/8
* CSS3 gradients and contrasts: pg 419/20

## Chapter 19: “Practical Information” (476-492)
* SEO = search engine optimization; how people find your site in the WWW
    * on page techniques:
        * page title
            * specified in < title >, which lives in < head >
        * url/web address
        * headings
            * if keywords are in < hm > elements, search engines will know that's what the site is about
        * text
            * keywords in the main body, at least 2-3 times
        * link text
            * link pages via text, no generic click here
        * image alt descriptions
            * will improve the chances of your images showing up on image-based searches 
        * page descriptions
            * lives inside the < head > element and is specified using a < meta > tag
            * it should be a sentence that describes the content of the page 
    * off-page techniques:
        * getting other sites to link to you
        * < a > tags in the link 
    * identifying keywords and phrases:
        * brainstorm: what would a person searching for your site type into google?
        * organize: group keywords into separate lists that live in differnt sections and categories of your website 
        * research: 
            * adwords.google.co.us/select/KeywordToolExternal
            * wordtracker.com
            * these are tools that might suggest additional keywords 
        * compare: what are other sites like yours doing? how tough is the competition?
        * refine: pick keywords you will focus on
            * if there is a keywords that generates a lot of competition, but is still very relevant to your site, use it 
        * map: pick 3-5 keywords or phrases that map each page of your website 
* google.com/analytics bayyyybeeee; consider:
    * how many people are coming to your website?
    * what are they looking at?
    * where are they from?
* domain name and hosting : pg 487/8
* FTP (file tranfer protocol) : pg 489/90
