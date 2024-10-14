## Two Key Aspects to Testing a Radio Button

**Functionality**: This aspect focuses on ensuring that the radio button functions correctly. Test cases under functionality testing may include verifying that only one option can be selected at a time, checking default selections, confirming proper labeling, and handling user interactions appropriately.

**Responsiveness**: The responsiveness aspect evaluates how the radio button displays and behaves under different conditions, such as varying screen resolutions or different user devices. It ensures that the radio button remains usable and visually appealing across a range of settings, contributing to a positive user experience.
___
#### Test Cases For Radio Buttons
- Verify that only one radio button can be selected at a time.
- Check if the radio buttons are initially unselected.
- Validate that clicking on the label associated with a radio button selects the button.
- Confirm that selecting one radio button deselects any previously selected option.
- Verify that keyboard navigation (e.g., using the “Tab” key) can select and deselect radio buttons.
- Test the behavior when no radio button is selected, and the form is submitted.
- Check if radio buttons maintain their state upon page refresh.
- Test the functionality of radio buttons with default pre-selected options.
- Verify the behavior of radio buttons with large labels or complex HTML structures.
- Validate radio button behavior when they are disabled (should not be selectable).
- Test radio button responsiveness at different screen resolutions (e.g., mobile, tablet, desktop).
- Test radio button behavior on touch devices to ensure easy selection.
- Verify the radio button’s appearance and functionality on various operating systems.
- Test the radio button under different network conditions to ensure it loads and responds efficiently.
- Check for visual consistency of radio buttons on different devices and browsers.
- Verify the radio button’s behavior when it is placed inside a radio button group with multiple sets of options.
- Test the radio button’s functionality in scenarios where there are more options than can fit within the visible viewport, ensuring proper scrolling or display mechanisms.
- Validate that radio buttons work correctly in multi-page forms, maintaining their selections as users navigate through the pages.
- Verify the radio button’s behavior when used in conjunction with other form elements, such as text fields or checkboxes, to ensure they do not interfere with each other.
- Check how radio buttons behave when used within complex forms with conditional logic or dynamic changes based on user selections.
___
#### Negative Test Scenarios for a Radio Button
- Attempt to select multiple radio buttons within the same group simultaneously.
- Try to select a radio button that is disabled.
- Test what happens when selecting a radio button with no options available in the group.
- Verify the behavior when pressing the “Enter” or “Space” key when the radio button is in focus but not selected.
- Check if the radio button maintains its selection after the page refresh.
- Attempt to submit a form with a required radio button not selected and verify the error message or validation response.
- Try to interact with radio buttons using keyboard shortcuts not associated with selection (e.g., “Ctrl” or “Alt” keys).