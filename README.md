
## Usage

```js
import Table from 'rc-table';

const columns = [
  {
    title: 'Name',
    dataIndex: 'name',
    key: 'name',
    width: 100,
  },
  {
    title: 'Age',
    dataIndex: 'age',
    key: 'age',
    width: 100,
  },
  {
    title: 'Address',
    dataIndex: 'address',
    key: 'address',
    width: 200,
  },
  {
    title: 'Operations',
    dataIndex: '',
    key: 'operations',
    render: () => <a href="#">Delete</a>,
  },
];

const data = [
  { name: 'Jack', age: 28, address: 'some where', key: '1' },
  { name: 'Rose', age: 36, address: 'some where', key: '2' },
];

React.render(<Table columns={columns} data={data} />, mountNode);
```
<!-- prettier-ignore -->
<table>
  <thead>
    <tr width="100%">
      <th>Name</th>
      <th>Author</th>
      <th>Descriptiopn</th>
      <th>Star</th>
    </tr>
  </thead>
  <tbody>
  <tr width="600px">
      <td>


</td>
<td>


</td>
</tr>

  </tbody>
</table>
## API

### Portfolio Template

| Name | Author | Default | Description |
| --- | --- | --- | --- |
| [Atail Template v.1.0.5](https://www.youtube.com/watch?v=j8WlpGy93Og) | [Themeforest](https://themeforest.net/) |  | key of this column |
| className | String |  | className of this column |
| colSpan | Number |  | thead colSpan of this column |
| title | React Node |  | title of this column |

## Summary Props

### Table.Summary

| Name | Type | Default | Description |
| --- | --- | --- | --- |
| key | String |  | key of this summary |
| fixed | boolean \| 'top' \| 'bottom' | - | `true` fixes the summary row at the bottom of the table. `top` fixes the summary row at the top of the table, while `bottom` fixes it at the bottom. `undefined` or `false` makes the summary row scrollable along with the table. |

### Table.Summary.Row

| Name | Type | Default | Description |
| --- | --- | --- | --- |
| key | String |  | key of this summary |
| className | String | - | className of this summary row |
| style | React.CSSProperties | - | style of this summary row |
| onClick | (e?: React.MouseEvent\<HTMLElement>) => void | - | The `onClick` attribute in `Table.Summary.Row` component can be used to set a click event handler for the summary row. |

## License

<table>
<tr>
<th align="center">
<img width="441" height="1">
<p> 
<small>
EXAMPLE TEXT
</small>
</p>
</th>
<th align="center">
<img width="441" height="1">
<p> 
<small>
EXAMPLE TEXT
</small>
</p>
</th>
</tr>
<tr>
<td>
<!-- REMOVE THE BACKSLASHES -->
\```jsonc
{
  "foo": [
    {
      "bar": "hello world"
    }
  ]
}
\```
  
</td>
<td>
<!-- REMOVE THE BACKSLASHES -->
\```jsonc
{
  "foo": [
    {
      "bar": "hello world"
    }
  ]
}
\```
  
</td>
</tr>
<tr>
<td align="center">
Column 1
</td>
<td align="center">
Column 2
</td>
</tr>
</table>
