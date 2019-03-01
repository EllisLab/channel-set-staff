# Staff Channel Set

Quickly create a Staff Channel in your ExpressionEngine install with this Channel Set.

The Staff Channel Set comes with custom fields to get you up and running fast. Here’s what’s inside:

### Custom Fields

* `{staff_biography}`: a Textarea for the staff member’s bio
* `{staff_email_address}`: an Email Address field for their email address
* `{staff_phone_number}`: a Text field for their phone number
* `{staff_position}`: a Text field for their position / job title

### Sample Tags

```
{exp:channel:entries channel='staff' order='title' sort='asc'}
	{if count == 1}
		<h1>Staff Members</h1>
		<ul>
	{/if}

			<li>
				<h2>{title}, {staff_position}</h2>
				<p>Email: {staff_email_address}<br>Phone: {staff_phone_number}</p>

				{staff_biography}
			</li>

	{if count == total_results}
		</ul>
	{/if}
{/exp:channel:entries}
```

## License

Copyright (C) 2004 - 2016 EllisLab, Inc.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL ELLISLAB, INC. BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Except as contained in this notice, the name of EllisLab, Inc. shall not be used in advertising or otherwise to promote the sale, use or other dealings in this Software without prior written authorization from EllisLab, Inc.
