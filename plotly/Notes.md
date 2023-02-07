These notes will be organized in the future


The **layout** is composed of a tree of "components" such as `html.Div` and `dcc.Graph`. It delcaritively describes the the app should look like

Dash **html components (dash.html)** contains a component class for every HTML tag as well as keyword args for all of the HTML arguments

# Callbacks

- **Callbacks** are functions that are automatically called by Dash `whenever an input component's property changes`, in order to `update some property in another component` (the output).

## **@app\.callback**
- Handles callback interactions between **HTML** and **Dash** components.
- In Dash, the `inputs` and `outputs` of our application are simply the properties of a particular component
```python
app.layout = html.Div([
	html.H6("Change the value in the text box to see callbacks in action!"),
	html.Div([
			  "Input: ",
			  dcc.Input(id='my-input', value='initial value', type='text')]),	
	html.Br(),
	html.Div(id='my-output'),
])

@app.callback(
	Input(component_id='my-input', component_property='value'),
	Output(component_id='my-output', component_property='children'))
	
def update_output_div(input_value):
	return f'Output: {input_value}'
```
- In the above code:
	- the input is the "`value`" property of the component that has the ID "`my-input`"
	- The output is the "`children`" property of the component with the ID "`my-output`"

- Whenever an `input property` changes, the function that the callback wraps will get called automatically