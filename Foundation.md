
Nền móng của Flexichat .....

Sử dụng thư viện, reacjs, ..
## Color

### Primary color
![[Primary color.png]]

#0082C9

Màu chính được lựa chọn cho giao diện là màu xanh và màu trắng.

>[!note]
>Quản trị viên có thể lựa chọn màu sắc chủ đề cho giao điện nhắn tin, người dùng cũng có thể thay đổi giao diện hiển thị theo ý thích.
>
- On web: `var(--color-primary-element)`
    
- Android: uses default Material Design colors
    
### Background color


|![[light.png]] <br><br>Background for light theme: #FFFFFF | ![[dark.png]]<br><br>Background for dark theme: #181818 |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

- On web: `var(--color-main-background)`
    
- Android: uses default Material Design colors
    
- iOS: [systemBackground](https://developer.apple.com/documentation/uikit/uicolor/3173140-systembackground)
    
- Desktop: [default Qt guidelines](https://doc.qt.io/qt-5/qpalette.html#ColorRole-enum)
    

### Text color[](https://docs.nextcloud.com/server/latest/developer_manual/design/foundations.html#text-color "Link to this heading")



|![../_images/colour-main-text.svg](https://docs.nextcloud.com/server/latest/developer_manual/_images/colour-main-text.svg)<br><br>Text in light theme: #222222[](https://docs.nextcloud.com/server/latest/developer_manual/design/foundations.html#id9 "Link to this image")|![../_images/colour-dark-theme-main-text.svg](https://docs.nextcloud.com/server/latest/developer_manual/_images/colour-dark-theme-main-text.svg)<br><br>Text in dark theme: #D8D8D8[](https://docs.nextcloud.com/server/latest/developer_manual/design/foundations.html#id10 "Link to this image")|

This is the main color for the text in light theme, and in dark theme.

- On web: `var(--color-main-text)`
    
- Android: uses default Material Design color “high emphasis”
    
- iOS: [label](https://developer.apple.com/documentation/uikit/uicolor/3173131-label) (in UITextView, leave the default textColor)
    
- Desktop: [default Qt guidelines](https://doc.qt.io/qt-5/qpalette.html#ColorRole-enum)
    

|   |   |
|---|---|
|![../_images/colour-text-maxcontrast.svg](https://docs.nextcloud.com/server/latest/developer_manual/_images/colour-text-maxcontrast.svg)<br><br>Secondary text in light theme: #767676[](https://docs.nextcloud.com/server/latest/developer_manual/design/foundations.html#id11 "Link to this image")|![../_images/colour-dark-theme-text-maxcontrast.svg](https://docs.nextcloud.com/server/latest/developer_manual/_images/colour-dark-theme-text-maxcontrast.svg)<br><br>Secondary text in dark theme: #8C8C8C[](https://docs.nextcloud.com/server/latest/developer_manual/design/foundations.html#id12 "Link to this image")|

In addition, a softer color is used for secondary text like sublines, timestamps, and similar.

- On web:`var(--color-text-maxcontrast)`
    
- Android: uses default Material Design color “medium emphasis”
    
- iOS: [secondaryLabel](https://developer.apple.com/documentation/uikit/uicolor/3173136-secondarylabel)
    
- Desktop: [default Qt guidelines](https://doc.qt.io/qt-5/qpalette.html#ColorRole-enum)
    

### Status and indicators[](https://docs.nextcloud.com/server/latest/developer_manual/design/foundations.html#status-and-indicators "Link to this heading")

|   |   |   |   |
|---|---|---|---|
|![../_images/color-info.svg](https://docs.nextcloud.com/server/latest/developer_manual/_images/color-info.svg)<br><br>Info: #006AA3[](https://docs.nextcloud.com/server/latest/developer_manual/design/foundations.html#id13 "Link to this image")|![../_images/color-success.svg](https://docs.nextcloud.com/server/latest/developer_manual/_images/color-success.svg)<br><br>Success: #46BA61[](https://docs.nextcloud.com/server/latest/developer_manual/design/foundations.html#id14 "Link to this image")|![../_images/color-error.svg](https://docs.nextcloud.com/server/latest/developer_manual/_images/color-error.svg)<br><br>Error: #E9322D[](https://docs.nextcloud.com/server/latest/developer_manual/design/foundations.html#id15 "Link to this image")|![../_images/color-warning.svg](https://docs.nextcloud.com/server/latest/developer_manual/_images/color-warning.svg)<br><br>Warning: #ECA700[](https://docs.nextcloud.com/server/latest/developer_manual/design/foundations.html#id16 "Link to this image")|

Interface elements associated with a status like info, success, error, or warning may also be colored to communicate the action better.

While interface elements like buttons are colored differently depending on their action, the color of the text in that element is almost always either of the main text colors, that is light or dark.

- On web:
    
    - Info color: `var(--color-info)`
        
    - Success color: `var(--color-success)`
        
    - Warning color: `var(--color-warning)`
        
    - Error color: `var(--color-error)`
        
- Android: Material Design guidelines
    
- iOS: [Apple HIG colors](https://developer.apple.com/design/human-interface-guidelines/ios/visual-design/color/)
    
    - success: systemGreen
        
    - error: systemRed
        
- Desktop: [default Qt guidelines](https://doc.qt.io/qt-5/qpalette.html#ColorRole-enum)
    

## Typography[](https://docs.nextcloud.com/server/latest/developer_manual/design/foundations.html#typography "Link to this heading")

[Penpot typography](https://design.penpot.app/#/view/db3839da-807b-8052-8002-576401e9a375?page-id=3f784c86-6c27-80c6-8002-6ab128f3ffe2&section=interactions&index=1&share-id=11fde340-21f4-802e-8002-8d8d305e7ab5)

To ensure compatibility with different platforms, Nextcloud apps always use the native system font.

For legibility, make sure that the text in your content uses:

- **Bold** for emphasis
    
- A line height between 130% and 150%
    
- The default tracking of the font
    
- No _italics_ or UPPER CASE as these text styles are less legible
    

The text sizes for the different platforms are:

- Web: 16px for main text and sublines, **20px bold** for headings
    
- Android: 14sp for main text, 16sp for headings
    
- iOS: values from [Dynamic Type Sizes, for size Large (Default)](https://developer.apple.com/design/human-interface-guidelines/ios/visual-design/typography#dynamic-type-sizes)
    
- Desktop: [default Qt guidelines](https://doc.qt.io/qt-5/qpalette.html#ColorRole-enum)
    

## Icons[](https://docs.nextcloud.com/server/latest/developer_manual/design/foundations.html#icons "Link to this heading")

[Penpot icons](https://design.penpot.app/#/view/db3839da-807b-8052-8002-576401e9a375?page-id=3f784c86-6c27-80c6-8002-6ab128f3ffe2&section=interactions&index=0&share-id=11fde340-21f4-802e-8002-8d8d305e7ab5)

![Material icons](https://docs.nextcloud.com/server/latest/developer_manual/_images/material-icons.png)

Icons can be used to communicate the intent of an action, or to provide visual interest to the screen. We use monochrome icons on all platforms: [Material Design icons (20 px default filled)](https://fonts.google.com/icons?icon.style=Filled&icon.set=Material+Icons) for web, Android, Windows and Linux, and [SF Symbols (default weight, scale and variant)](https://developer.apple.com/sf-symbols/) for iOS and macOS.

This is except for the icon of the app itself, which can be a custom icon.

Make sure to:

- Not overuse icons
    
- When possible, use text together with icons so it’s clear what they refer to
    
- For special cases like warnings, combine the icon with color to enhance its visibility
    

## Naming[](https://docs.nextcloud.com/server/latest/developer_manual/design/foundations.html#naming "Link to this heading")

To be immediately understandable, we choose app names which are generic and easily translatable. Additionally, they are short and easily fit in the top navigation without being cut off.

Files, Contacts, Calendar, and Mail do not need further explanation, which is why we recommend to choose a self-explanatory app name.

Further good examples of this: Notes, Bookmarks, Maps, Forms, Tasks, Music.

## Wording[](https://docs.nextcloud.com/server/latest/developer_manual/design/foundations.html#wording "Link to this heading")

The wording and language in your app sets the tone and approachability of your app.

- Nextcloud should always be written out, and only with a capital N. Not “NextCloud” or “Nc”.
    
- Be friendly and approachable, not condescending.
    
- Use understandable language, not technical jargon. For example, “link” is much better than “URL”, and explaining errors is better than showing error codes.
    
- Don’t write in ALL CAPS, as it is not as readable and comes off as shouting and aggressive. Also use Sentence case and not Capital Case, with the exception of product names like Nextcloud Talk, Nextcloud Hub, etc.
    
- We are a community, so better write “We are happy to announce” instead of “I am happy to announce”.
    
- If your app content is empty, it can be helpful to add an engaging message. “Add or import your first bookmark!” is much nicer than “No bookmarks yet”.
    
- Try to avoid using “my” or “your” like in “My files” or “Your files”, instead using “All files”. For longer sentences where it cannot be avoided, use “your”, never “my”.
    
- Use gender neutral language. This [international guide to gender-inclusive writing](https://uxcontent.com/the-international-guide-to-gender-inclusive-writing/) contains info and examples on gender neutral wording for different languages.
    
- Use full names instead of only first names while addressing the person using your app.
    
- For any “Delete” action, give context to what it will delete, like “Delete conversation” or “Delete user” so that it is clear specifically for this destructive action.
    
- Keep language short and concise, and keep in mind that it should be easily translatable.
    
- Make sure to spellcheck anything you write.