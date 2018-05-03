# Default Mappings

**! NOTE: This document is currently a work in progress !**

These are the "rules" that are used to create the mappings in the default profiles.

Types are matched exactly but without case-sensitivity.
Names are matched based on the proerty name containing the value specified and without case-sensitivity.
The order of items is in the tabel does not reflect the order in which 

## UWP

| Property Type  | Is Read-only | Property Name | Control          | Other Attributes/Notes           |
|----------------|--------------|---------------|------------------|----------------------------------|
| **{fallback}** | _n/a_        | _n/a_         | TextBlock        |                                  |
| String         | false        | -             | TextBox          |                                  |
| String         | **TRUE**     | -             | TextBlock        |                                  |
| String         | **TRUE**     | uri/url       | HyperlinkButton  |                                  |
| String         | false        | uri/url       | TextBox          | InputScope="Url"                 |
| String         | false        | phone/tel     | TextBox          | InputScope="TelephoneNumber"     |
| String         | false        | email         | TextBox          | InputScope="EmailNameOrAddress"  |
| String         | false        | firstname/lastname/<br />familyname/surname/<br />givenname | TextBox | InputScope="PersonalFullName" |
| String         | false        | password      | PasswordBox      |                                  |
| String         | false        | search        | AutoSuggestBox   |                                  |
| int/Integer    | **TRUE**     | -             | TextBlock        |                                  |
| ICommand<br />Command<br />RelayCommand | false | - | Button     |                                  |
| DateTimeOffset | false        | -             | DatePicker       |                                  |
| bool/Boolean   | false        | -             | ToggleSwitch     |                                  |
| bool/Boolean   | false        | isbusy/isactive | ProgressRing   |                                  |
| Uri            | **TRUE**     | -             | HyperlinkButton  |                                  |
| List&lt;string&gt; | false    | -             | ItemsControl     |                                  |
| ObservableCollection&lt;T&gt;<br />List&lt;T&gt; | false | -  | ListView |                          |
| enum           | false       | -              | RadioButton [*](https://github.com/Microsoft/Rapid-XAML-Toolkit/issues/58) |   |
|                |             |                |                  |                                  |

## WPF

**TBD **

| Property Type  | Is Read-only | Property Name | Control          | Other Attributes/Notes           |
|----------------|--------------|---------------|------------------|----------------------------------|
| **{fallback}** | _n/a_        | _n/a_         | TextBlock        |                                  |
|                |              |               |                  |                                  |
|                |              |               |                  |                                  |
|                |              |               |                  |                                  |

## Xamarin.Forms

| Property Type  | Is Read-only | Property Name | Control          | Other Attributes/Notes           |
|----------------|--------------|---------------|------------------|----------------------------------|
| **{fallback}** | _n/a_        | _n/a_         | Label            |                                  |
| String         | **TRUE**     | -             | Label            |                                  |
| String         | false        | -             | Entry            |                                  |
| String         | false        | password/pwd  | Entry            | IsPassword="True"                |
| String         | false        | search        | SearchBar        | Placeholder="Search"             |
| String         | false        | phone/tel     | Entry            | Keyboard="Telephone"             |
| String         | false        | chat/message  | Entry            | Keyboard="Chat"                  |
| String         | false        | email         | Entry            | Keyboard="Email"                 |
| String         | false        | uri/url       | Entry            | Keyboard="Url"                   |
| String         | false        | int/Integer/long/<br />double/float | Entry | Keyboard="Numeric"    |
| DateTimeOffset/<br />DateTime | false | date  | DatePicker       |                                  |
| DateTimeOffset/<br />DateTime | false | time  | TimePicker       |                                  |
| ICommand<br />Command<br />RelayCommand | false | - Buutton      |                                  |
| List&lt;string&gt; | false    | -             | Picker           |                                  |
| ObservableCollection&lt;T&gt;<br />List&lt;T&gt; | false | -  | ListView |                          |
|                |              |               |                  |                                  |