# Accessibility

## Structure & hierarchy

Consistent, clear hierarchy helps users who navigate the page using links or headers. Use headings and titles to outline the page so that users can see the structure and how the sections relate. Give users feedback so they know where they are in the application.

## Meaningful text

Consistent and helpful text makes the user interface accessible to users who use a screen reader. Screen readers help users with visual impairments by reading both visible and non-visible alternative text aloud.

All text should support accessibility, whether it's visible \(UI labels, headings, buttons, forms, hyperlinks, and help text\) or non-visible \(alternative text for images and buttons\).



### Be concise

Keep content and accessibility text concise. People using screen readers hear every UI element read aloud, so the shorter the text, the faster they can navigate the content.

### Use consistent labels 

Consistently label elements and components that have the same functionality. When users encounter these elements in different contexts, they should be able to easily recognize and understand the function or actions of an element. For instance, a menu item that is labelled _All sprints_ should open a page that is titled _All sprints_. A dialogue with the title _Copy page_ has a button labeled _Copy_.

* **Do:** Copy a ticket, copy a page
* **Don't:** Clone a ticket, copy a page

### Describe what an element does

Label elements with action verbs that indicate what happens when the element is selected.

* **Do:** Edit preferences - When read aloud, the text indicates the action. 
* **Don't:** Preferences - Just labeling the element doesn't let the user know what will happen when it is selected.

In buttons, describe what the action does, and, if you can, reveal what will happen.

* **Do:** Add room
* **Don't:** Go for it! 

Hyperlinks indicate where the user will go when they select the link.

* **Do:** Learn more about Jira permissions
* **Don't:**Read more

## Images and video

Describe non-text elements in the UI or with alternative text so that screen readers can succinctly describe images and media.

### Images that contain information

If an image contains information that can only be understood by seeing the image, then you need to explain the content of the image using alternative text. Follow these guidelines when you write alt text:

* The text should be an adequate replacement for both the content and the function of the image. 
* Determine the correct content and then deliver that message as succinctly as possible. Aim for no more than a few words, though sometimes a short sentence or two may be necessary.
* Don't repeat information that is contained in the text found on the page around the image. 
* Don't use phrases like "image of ..." or "a photo of ..." to describe the image. This is apparent when using screen readers and the description itself should be enough to replace the meaning of the image. 
* If the meaning and content of an image is conveyed by surrounding text, header, or captions, then you might not need as much alternative text.

### Decorative images

If the image is used strictly to make the page pleasant to the eye, doesn't contain a link, and isn't used to deliver information, then include the alt attribute, but leave it empty. For example, _alt=""_

### Videos

Provide transcripts and in-sync captioning. Make sure users can control when the video or gif starts and stops.  


## Colors

We comply with [AA standard contrast ratios](http://www.w3.org/TR/WCAG/). To do this, we choose primary, secondary and extended colors that support usability. This ensures sufficient color contrast between elements so that users with low vision can see and use our products.

### Include visual cues

Don't convey information using color alone. Use multiple visual cues, such as stroke weight, patterns, shape, text, or illustrations to ensure that all users receive the same information.

This helps users who are unable to, or have difficulty with, distinguishing one color from another. This includes people who are color blind, have low vision, or are blind.

### Use high contrast

High color contrast helps users who are partially or completely color-blind see differences between certain colors. It creates a strong visual hierarchy and improves usability for everyone. Make sure that the combination of text and background color do not fall below the [WCAG recommended threshold](https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-contrast.html) ratio of 4.5:1 for standard text and 3:1 for larger text.

Decorative images and disabled states don't have contrast requirements.

