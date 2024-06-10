# react select menu component

## Installation

```bash
npm i select-menu-oc-p14
```

## Props needed

- `label`: label text displayed above the select menu

- `data` : array of objects to be displayed in the select menu

- `labelKey` : key to be displayed as label in the select menu

- `valueKey` : key to be used as value in the select menu

- `value` : value of the selected option

- `rest` : additional props to be passed to the select menu

## Example

```jsx
import SelectMenu from 'select-menu-oc-p14';

function App() {
  const departments = [
    {
      department: 'Sales',
    },
    {
      department: 'Marketing',
    },
  ];

  const states = [
    {
      name: 'Alabama',
      abbreviation: 'AL',
    },
    {
      name: 'Alaska',
      abbreviation: 'AK',
    },
  ];
  return (
    <div className='flex h-screen items-center justify-center gap-5'>
      <h1 className='text-2xl font-bold text-white'>Select Menu</h1>
      <SelectMenu
        label='Departments'
        data={departments}
        valueKey='department'
        labelKey='department'
      />

      <SelectMenu
        label='States'
        data={states}
        valueKey='abbreviation'
        labelKey='name'
      />
    </div>
  );
}

export default App;
```
