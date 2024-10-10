
# Website Accessibility Test Report

**Website:** https://www.srf.ch/
**Date:** 10.10.2024
**Tester:** Kai Tran & Josua Bürki

<hr />

## 1. **Perceivable**

### 1.1. **Text Alternatives**

- **1.1.1 Non-text Content:**

  *Tested:* All non-text content that is presented to the user has a text alternative that serves the equivalent purpose, except for the situations listed below. 

  *Observations:* The images on the home page don't have an alternative text

  *Result:* Failed.

### 1.2. **Time-based Media**

- **1.2.1: Audio-only and Video-only (Prerecorded)**

  *Tested:* For prerecorded audio-only and prerecorded video-only media, the following are true, except when the audio or video is a media alternative for text and is clearly labeled as such: 

  *Observations:* Yes, all the articles have a corresponding video or audio file.

  *Result:* Passed.

- **1.2.2: Captions (Prerecorded)**

  *Tested:* Captions are provided for all prerecorded audio content in synchronized media, except when the media is a media alternative for text and is clearly labeled as such. 

  *Observations:* No, none of the videos or audio files have a caption

  *Result:* Failed.

- **1.2.4: Captions (Live)**

  *Tested:* Captions are provided for all live audio content in synchronized media. 

  *Observations:* SRF also has live radio on it's website but it doesn't provides caption.

  *Result:* Failed.

- **1.2.5: Audio Description (Prerecorded)**

  *Tested:* Audio description is provided for all prerecorded video content in synchronized media.

  *Observations:* The videos don't have a audio description.

  *Result:* Failed.

### 1.3. **Adaptable**

- **1.3.1 Info and Relationships:**

  *Tested:* Information, structure, and relationships conveyed through presentation can be programmatically determined or are available in text.

  *Observations:* SRF doesn't fulfil this completely. Inside an article, it uses h1 and paragraphs but on the home page, all the text is insed span's and it's not clear what is the title, subtitle and text.

  *Result:* Failed.

- **1.3.4 Orientation:**

  *Tested:* Content does not restrict its view and operation to a single display orientation, such as portrait or landscape, unless a specific display orientation is essential.

  *Observations:* All the content is developped for mobile and web this portrait and landscape mode.

  *Result:* Passed.

- **1.3.4 Orientation:**

  *Tested:* The purpose of each input field collecting information about the user can be programmatically determined when:

  *Observations:* There is only a search bar and a contact form, both have label-input and reasonable descriptions.

  *Result:* Passed.

### 1.4. **Distinguishable**

- **1.4.1 Use of Color:** 

  *Tested:* Color is not used as the only visual means of conveying information, indicating an action, prompting a response, or distinguishing a visual element.

  *Observations:* No color is never used to convey information or indicating an action, it is always combined with shape and text/icon.

  *Result:* Passed.

<hr />

## 2. **Operable**

### 2.1. **Keyboard Accessible**

- **2.1.1: Keyboard**

  *Tested:* All functionality of the content is operable through a keyboard interface without requiring specific timings for individual keystrokes, except where the underlying function requires input that depends on the path of the user's movement and not just the endpoints.

  *Observations:* Yes the user can interact with the website via the keyboard i.e. can use the "tab" button to hop to the next element and "enter" to select it (same as click)

  *Result:* Passed.

- **2.1.2: No Keyboard Trap**

  *Tested:* If keyboard focus can be moved to a component of the page using a keyboard interface, then focus can be moved away from that component using only a keyboard interface, and, if it requires more than unmodified arrow or tab keys or other standard exit methods, the user is advised of the method for moving focus away.

  *Observations:* All components I observed were accessibel by "tab" and user could get back via "shift" + "tab".

  *Result:* Passed.

### **2.3 Seizures and Physical Reactions**

- **2.3.1: Three Flashes or Below Threshold**

  *Tested:* Web pages do not contain anything that flashes more than three times in any one second period, or the flash is below the general flash and red flash thresholds.

  *Observations:* No, didn't finde anything

  *Result:* Passed.

### **2.4 Navigable**

- **2.4.2: Page Titled**

  *Tested:* Web pages have titles that describe topic or purpose.

  *Observations:* Yes, all except the home page

  *Result:* Passed.

- **2.4.3: Focus Order**

  *Tested:* If a Web page can be navigated sequentially and the navigation sequences affect meaning or operation, focusable components receive focus in an order that preserves meaning and operability.

  *Observations:* Yes it generally makes sense, from the top left to the bottom right, row by row. Only in the weather forecast where there are multiple cities on a map, they are in a random order, but there isn't a true order anyway in this case.

  *Result:* Passed.

- **2.4.4: Link Purpose (In Context)**

  *Tested:* The purpose of each link can be determined from the link text alone or from the link text together with its programmatically determined link context, except where the purpose of the link would be ambiguous to users in general.

  *Observations:* Yes it can.

  *Result:* Passed.

<hr />

## 3. **Understandable**

### 3.1. **Readable**

- **3.1.1 Language of Page:**

  *Tested:* The default human language of each Web page can be programmatically determined.

  *Observations:* Yes in the html tag the lang is defined.

  *Result:* Passed.

- **3.1.2: Language of Parts**

  *Tested:* The human language of each passage or phrase in the content can be programmatically determined except for proper names, technical terms, words of indeterminate language, and words or phrases that have become part of the vernacular of the immediately surrounding text.

  *Observations:* The entire content is in german and therefore this never occurs thus passed

  *Result:* Passed.

### **3.2. Predictable**

- **3.2.1: On Focus**

  *Tested:* When any user interface component receives focus, it does not initiate a change of context.

  *Observations:* If I understand this correctly, all the links open in the same tab and window, so it doesn't violate this guideline

  *Result:* Passed.

### 3.3. **Input Assistance**

- **3.3.1 Error Identification:**

  *Tested:* If an input error is automatically detected, the item that is in error is identified and the error is described to the user in text.

  *Observations:* There is no input mechanism on the page except the contact form and all the required but unfilled fields are highlighted red

  *Result:* Passed.

- **3.3.2: Labels or Instructions**

  *Tested:* Labels or instructions are provided when content requires user input.

  *Observations:* Yes, as said the form

  *Result:* Passed.

<hr />

## 4. Robust

### 4.1. Compatible

- **4.1.1: Parsing**

  *Tested:* In content implemented using markup languages, elements have complete start and end tags, elements are nested according to their specifications, elements do not contain duplicate attributes, and any IDs are unique, except where the specifications allow these features.

  *Observations:* Yes, all elements have complete start and end tags and are nested correctly.

  *Result:* Passed.

- **4.1.2 Name, Role, Value:**

  *Tested:* For all user interface components (including but not limited to: form elements, links and components generated by scripts), the name and role can be programmatically determined; states, properties, and values that can be set by the user can be programmatically set; and notification of changes to these items is available to user agents, including assistive technologies.

  *Observations:* Yes they do, but sometimes a bit cryptic

  *Result:* Passed.

<hr />

## Conclusion

The website shows strong accessibility, passing 17 out of 22 WCAG criteria. It is user-friendly designed and has a clear structure contributing to a positive user experience for everyone.