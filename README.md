
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

## API

### Portfolio Template

| Name | Author | Default | Description |
| --- | --- | --- | --- |
| [Atail Template v.1.0.5](https://www.youtube.com/watch?v=j8WlpGy93Og) | String |  | key of this column |
| className | String |  | className of this column |
| colSpan | Number |  | thead colSpan of this column |
| title | React Node |  | title of this column |
| dataIndex | String |  | display field of the data record |
| width | String \| Number |  | width of the specific proportion calculation according to the width of the columns |
| fixed | String \| Boolean |  | this column will be fixed when table scroll horizontally: true or 'left' or 'right' |
| align | String |  | specify how cell content is aligned |
| ellipsis | Boolean |  | specify whether cell content be ellipsized |
| rowScope | 'row' \| 'rowgroup' |  | Set scope attribute for all cells in this column |
| onCell | Function(record, index) |  | Set custom props per each cell. |
| onHeaderCell | Function(record) |  | Set custom props per each header cell. |
| render | Function(value, row, index) |  | The render function of cell, has three params: the text of this cell, the record of this row, the index of this row, it's return an object:{ children: value, props: { colSpan: 1, rowSpan:1 } } ==> 'children' is the text of this cell, props is some setting of this cell, eg: 'colspan' set td colspan, 'rowspan' set td rowspan |

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

rc-table is released under the MIT license.
