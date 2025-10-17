# **HL7 v2.x Message Editor**

A powerful, single-file, web-based tool for parsing, viewing, editing, and validating HL7 v2.x messages. Built with modern HTML5, JavaScript, and Tailwind CSS, this editor provides a rich user experience for healthcare IT professionals, developers, and analysts working with HL7 data.

## **Features**

* **Flexible Input Methods:**  
  * **Paste:** Directly paste raw HL7 message text.  
  * **File Open:** Open local .hl7 or .txt files.  
  * **Drag & Drop:** Drag and drop message files directly onto the editor.  
  * **Templates:** Start with common message templates like ADT^A01, ORM^O01, and ORU^R01.  
* **Advanced Parsing:**  
  * Automatically parses segments, fields, components, and sub-components.  
  * Correctly handles custom delimiters defined in the MSH segment.  
  * Specialized logic for MSH segment indexing.  
* **Interactive Dual-View Display:**  
  * **Raw View:** A color-coded, clickable representation of the raw HL7 message.  
  * **Structured View:** A collapsible, tree-like view of the message structure.  
  * **Synced Highlighting:** Clicking on an element in one view highlights the corresponding element in the other.  
* **Detailed Element Inspector:**  
  * Select any field, component, or sub-component to view its details.  
  * Displays the element's path (e.g., PID-5.2), official HL7 description, and current value.  
  * Provides a breakdown of components and sub-components with their defined names from the internal HL7 dictionary.  
* **Live Editing & Version Control:**  
  * Edit any part of the message in the "Details" panel.  
  * Changes are only committed when you click **Apply**.  
  * Instantly **Undo** any typed changes before applying.  
  * All views (Raw, Structured, and Details) are instantly and consistently updated upon applying a change.  
* **Rich Data Dictionary:**  
  * Includes a comprehensive internal dictionary for common HL7 segments (MSH, PID, PV1, OBX, etc.), fields, components, and sub-components.  
  * Displays descriptive names for message types and trigger events.  
* **User Experience Enhancements:**  
  * **Dark Mode:** Toggle between light and dark themes. Remembers your preference.  
  * **Collapsible Segments:** Easily collapse and expand segments in the structured view to manage large messages.  
  * **Responsive Design:** Fully functional on desktop and mobile browsers.  
* **Export Functionality:**  
  * Export your edited message as a valid .hl7 file.

## **Technologies Used**

* **HTML5:** For the core structure of the application.  
* **Tailwind CSS:** For a modern, responsive, and utility-first styling approach.  
* **JavaScript (ES6+):** For all parsing, DOM manipulation, and interactive features. No external libraries are required.

## **How to Use**

1. Download the index.html file.  
2. Open the file in any modern web browser (Chrome, Firefox, Safari, Edge).  
3. You can now:  
   * Paste an HL7 message into the "Raw HL7 Input" box.  
   * Click "Open File" to load a message from your computer.  
   * Drag and drop a file onto the input box.  
   * Select a message from the "Message Templates" dropdown to get started.

The message will be parsed automatically, and you can begin exploring and editing its contents.

## **Future Enhancements**

This project has a solid foundation with room for more features:

* **Real-time Validation:** Add logic to validate fields, data types, and lengths against the HL7 standard as the user edits.  
* **Segment/Field Creation:** Allow users to add new segments, fields, or repetitions to an existing message.  
* **Message ACK Generation:** Automatically generate an ACK message in response to the loaded message.  
* **Search Functionality:** Implement a search bar to quickly find specific values or segments within the message.

