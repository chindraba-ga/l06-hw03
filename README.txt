l06-hw03
* Status: Submitted
* CodePen: <https://codepen.io/chindraba-ga/pen/oNxYZgG>
* Live page: <https://www.chindraba.work/fewd/l06-hw03.html>

Contents
================================================================================

* Description
* Copyright and License
  * The MIT License

Description
================================================================================

Lesson 6: Assignment: Rebuild a page from Trulia

Now you're stepping into the big leagues - you'll be rebuilding part of a real website: trulia.com

We will still give you content and colors and fonts like the last assignment, but this is much more difficult. You will need to consider how to do this layout before diving in.

The starter code is:

- HTML

    ## Reference content

    ### Font
    Lato 400 Regular
    https://fonts.google.com/?category=Sans+Serif&selection.family=Lato

    ### Navigation:
    Buy Rent Mortgage Local Scoop
    Saved Homes Saved Searches jsir

    ### Houses:

    $475,000
    2bd
    2ba
    715 sqft
    3205 Georgia Ave NW #403
    Pleasant Plains, Washington, DC

    $774,900
    2bd
    3ba
    3615 10th St NW #8
    Columbia Heights, Washington, DC

    $600,000
    3 bd
    2 ba
    3120 Park Pl NW
    Pleasant Plains, Washington, DC

    $630,000
    2bd
    3ba
    1500 sq ft
    3221 Warder St NW #1
    Pleasant Plains, Washington, DC

    $1,295,000
    9bd
    6ba
    705 Kenyon St NW
    Pleasant Plains, Washington, DC

    $1,049,000
    6bd
    4ba
    2688 sqft
    1363 Oak St NW
    Columbia Heights, Washington, DC

    $720,000
    3bd
    3ba
    1850 sqft
    1307 Irving St NW #1
    Columbia Heights, Washington, DC

    $760,000
    3bd
    3ba
    1920 sqft
    752 Park Rd NW
    Columbia Heights, Washington, DC

    $760,000
    3bd
    3ba
    1920 sqft
    752 Park Rd NW
    Columbia Heights, Washington, DC

    $999,000
    2bd
    4ba
    2395 sqft
    3511 17th ST NW #7
    Mount Pleasant, Washington, DC

    $474,500
    2bd
    1ba
    964 sqft
    1356 Kenyon St NW #8
    Columbia Heights, Washington, DC

    $399,000
    1bd
    1ba
    462 sqft
    3205 Georgia Ave NW, #505
    Pleasant Plains, Washington, DC

    ### Images: 

    Logo:
    https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/logo.svg

    House pics:
    https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/house-1.jpg
    https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/house-2.jpg
    https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/house-3.jpg
    https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/house-4.jpg
    https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/house-5.jpg
    https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/house-6.jpg
    https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/house-7.jpg
    https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/house-8.jpg
    https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/house-09.jpg
    https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/house-10.jpg
    https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/house-11.jpg
    https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/house-12.jpg

    Icons
    https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/bed-icon.png
    https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/bath-icon.png

    Arrows:
    https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/down-arrow-outline.svg
    https://s3-us-west-2.amazonaws.com/s.cdpn.io/2522641/up-sign.svg

    ### Footer:

    1 2 3 4 >
    1 - 30 of 79 Results
    United States > District Of Columbia > Washington > 20010

    20010 Real Estate Insights
    ZIP code 20010 is located in Washington, District of Columbia.

    The plethora of grocery stores in ZIP code 20010 makes it easy to stock up on specialty foods, like organic and gluten-free options, without having to leave the area. There is easy access to public transportation [https://www.trulia.com/real_estate/20010-Washington/], which is the preferred way to travel here due to its ease of use and abundant travel options. Bicycles are big sellers in ZIP code 20010; everyone seems to be riding these days, whether it's for the daily commute or a fun afternoon with the family.

    Many houses in ZIP code 20010 are historic with one-of-a-kind architecture, and it's clear to see why it's so important to maintain them and keep history living on. This year, the average listing price grew to $658,471  in this locale, a noticeable appreciation of 12.5 percent from $585,528 the year prior. During the same period, inventory is noticeably increasing in this locale year-over-year, with a 20 percent increase in for-sale listings last year alone. Enjoy a cozy night by the fire, as many residences here come equipped with authentic fireplaces. ZIP code 20010 has some great historic estates so if you move to one of these homes, you'll be inheriting a piece of history. If you enjoy a view and the ability to see far and wide, consider a penthouse in this place [https://www.trulia.com/for_sale/20010_zip/penthouse_keyword/] for an unparalleled experience.

    HTML Skeleton to get you going:
    <main class="trulia-grid">

        <!-- Example grid-item -->
        <section class="trulia-grid-item">
          <div class="trulia-house-image">
            <img src="#" alt="">
          </div>
          <ul class="trulia-house-facts">
            <li class="trulia-house-price"></li>
            <li class="trulia-house-stats">
              <ul>
                <li class="trulia-house-beds-icon"></li>
                <li class="trulia-house-beds"></li>
                <li class="trulia-house-baths-icon"></li>
                <li class="trulia-house-baths"></li>
                <li class="trulia-house-sqft"></li>
              </ul>
            </li>
            <li class="trulia-house-address">
            </li>
            <li class="trulia-house-location">
            </li>
          </ul>
        </section>
      
      </main>

- CSS

    ### Colors
    Green: #20c063 / RGBA(32,192,99,1)
    Gray: #e8e9ea  / RGBA (232,233,234,1)
    Dark Text: #3b4144 / RGBA (59,65,68,1)


Copyright and License
================================================================================

The MIT license applies to all the code within this repository.

Copyright © 2020  Chindraba (Ronald Lamoreaux)
            <upskill@chindraba.work>
- All Rights Reserved

The MIT License

Permission is hereby granted, free of charge, to any person obtaining a
copy of this software and associated documentation files (the "Software"),
to deal in the Software without restriction, including without limitation
the rights to use, copy, modify, merge, publish, distribute, sublicense,
and/or sell copies of the Software, and to permit persons to whom the
Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included
in all copies or substantial portions of the Software

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGE MENT. IN NO EVENT SHALL
THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
DEALINGS IN THE SOFTWARE.
