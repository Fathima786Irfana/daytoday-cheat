# Factory class Cheat Sheet
In the configurator (conf), we define an **`action`** field that can contain various actions like `Onload`, `Onchange`, `Add Row`, `Edit Details`, etc.
Each action needs to perform a **distinct set of operations**. To handle this dynamically, we use a **factory class** that maps each action to a specific handler class.
This ensures that the correct logic is executed for each action mentioned in the configurator.
|  pos  | Action        |
|-------|---------------|
| 10    | Add Row       |
| 20    | Edit Details  |
| 30    | Onchange      |
Each action is tied to a position (`pos`) and executed accordingly.
### Basic Factory Class Syntax
```javascript
class  clActionFactory {
	private  static  actionsMap: {
	[key:  string]:  new (iAction:  string, iaActionData:  TTactionsData) =>  clAction } = {
	"Onload":  clActionOnLoad,
	"On Change":  clActionOnChange,
	"On Tab":  clActionOnTab,
	"Add Row":  clActionAddRow,
	"Edit Details":  clActionEditDetails,
	"Expand Section":  clActionExpandSection,
	};
```