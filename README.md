# Smart-Image-Classifier


In my model, I used Writing Tools as a BaseLine. I made three classes- Pencils, Black Pens, and Colored Pens. Here's how I captured all my photoes:

| Category | Details |
|---|---|
| Where | I took some photos in my apartment and some at work. |
| Lighting | I used a mix of warm lighting, dark lighting, and direct light. |
| Background | I used paper, notebooks, a desk, and a counter as surfaces. |
| Distance | I took some photos from far away and some close up. |
| Angles | Most of my photos were straight-on, but a few were at an angle. |
| Hands/Objects | I had my hands in a few of the photos, but usually paper or other items were present. |

After trining my model, I would say it was most condifent in its ability to tell what type on Pen was present- if it was black, or colorful. Out of 15 test images, it scored a 13/15! However, I don't believe it was fully accurate. Some of the test images I put through weren't pens...rather, they were markers- which is where I think my model has a slight flaw in telling the differences in shape. 

| Test | Score | Observation |
|---|---|---|
| Part 2 Baseline | 10/15 | It seemed to focus more on the grass from the photos taken outside than on the pen. |
| Different Place | 14/15 | It recognized the pen in the photo. |
| Different Light | 5/15 | It mistook most of the colorful pens for black pens in different lighting. The colors were less saturated in these photos. |
| Different Distance | 8/15 | It recognized some pens, but the distance and slight blur in some photos seemed to trip up the model. |
| Someone Else's | 7/15 | It could read some pens, but it did not recognize pens that did not look like typical pens, such as character pens. |

After running the rouge tests- the colors seemed to trip my Model up the most. Applying different color filters to some photos caused my model to have a 80% accuracy, down to a around 53%. Of all the tests I ran, the different lighting seemed to be the biggest impact to my model- as I said before, the changes in light effected the ability for the model to tell what colors were being shown. So it either didn't guess correctly or just couldn't figure it out at all.
    Once I changed it to recognize different lighting settings- it seemed to peform a lot better. Rather than getting a 53% over all- it managed to bump up to a 76%. While stillnot totally accurate, it still performed better than it did previosuly without the changes! Some colors still tripped up the model (notably cooler tones like blue and purple in my models case) where as warmer colors seemed to pass through easier. (Since warmer tones can often be associated with common indoor lighting). 