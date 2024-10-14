1. Keyboard Navigation Testing - all content is avaialble via keyboard, there's visible focus indicator, non-interactive elements don't recieve focus
    - using keyboard
    - using bluetooth keyboard with a tablet
    - using bluetooth keyboard with a tablet when the screen reader is on
    - using sreen reader and a keyboard
2. Contrast Testing
    - high contrast is available
3. Screen Reader Testing (JAWS, NVDA, VoiceOver, TalkBack)
    - any text
    - info about an interactive element
    - pictures
    - pop-up  
        A. There are diff mode for readers:
    - Browse Mode/Read
    - Forms Mode
    - Application Mode

---
### Tools:
##### Online tools:
1. Nu HTML Checker (W3C)
2. CSS Validation Service (W3C)
3. AChecker
4. WAVE
##### Browser tools
1. AInspector Sidebar
2. WAVE
3. axe
4. ARC Toolkit
5. Accessibility Insights for Web
___
### Check-list

Main questions:

- Можно ли при помощи клавиатуры выполнить те же действия, которые выполняются с мышью?
- Есть ли соответствующие инструкции в документации или руководстве пользователя?
- Логично ли расположены вкладки? (Это способствует плавной навигации).
- Есть ли комбинации клавиш для работы с меню?
- Все ли метки в приложении подписаны правильно?
- Правильно ли используются картинки и иконки, т. е. легко ли их понять конечному пользователю?
- Может ли пользователь перезаписать дефолтные шрифты для вывода текста на экран?
- Может ли пользователь отключить или ограничить мигание и движение на экране?

Radio button should provide:

- function of check and move through options by keyboard
- have clear and simple label
- use native tag into html `<fieldset><label><input type= name= value=></label>`
- use ARIA technique
- contrast icon 3:1
- contrast text label 4.5:1
- text spacing
- focus indicator should be visible

### Tools

1. Wave
2. TAW
3. Accessibility Valet
4. Accessibility Developer Tools
___
[Web Accessibility testing toolkit.pdf](file:///C:/Users/Artsemi_Vadalazau/.config/joplin-desktop/resources/b931af086ac5497bb418f2993b4dd1d3.pdf "file:///C:/Users/Artsemi_Vadalazau/.config/joplin-desktop/resources/b931af086ac5497bb418f2993b4dd1d3.pdf")  
