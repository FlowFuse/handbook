## Contributing to the Handbook

As mentioned in our [introduction](/handbook/#about-the-handbook), we strongly encourage anyone working
at FlowForge to contribute to the Handbook. In fact, FlowForge operates with the policy that
["Everybody Codes"](/handbook/company/policy#everybody-codes), and with that, every employee should
feel empowered to contribute to any of our code bases.

The handbook is a good entry-level code base to get started with, it's driven by
<a href="https://www.markdownguide.org/basic-syntax/" target="_blank">Markdown</a> (`.md`) files, which are easy
to read and understand, for example:

    # this is a title

    This is text after the title with a [link](https://example.com) in it

The handbook is <a href="https://github.com/flowforge/handbook" target="_blank">maintained on GitHub</a>
and contributions can be made through "pull-requests".

If you're new to Git, we have an [entry-level guide](/handbook/development/contributing/git-how-to) on how
to get started which walks through creating an editing `.md` files as an example.

### Handbook Navigation

When the Handbook is built into the Website, it will automatically work out the navigation hierarchy,
as you'll see on the left-hand side here.

For example, this file lives in the `/development/contributing/` folder, and so, that's where it
lives in the side navigation.

#### Custom Labels

The label for a given page is automatically generated from the file name. For example, if the file
is called `handbook.md`, then it will appear as "Handbook" in the navigation menu.

Let's say we have another file though, `git-how-to.md`, which would automatically render
as "Git-How-To" in the menu. If you want to change this label, or make it easier to read,
you can add:

    ---
    navTitle: Using Git
    ---

at the top of your `.md` file, and the side navigation will use this label instead.

#### Adding Folders

If you're adding a new folder into the Handbook, please include an `index.md` file within that folder,
e.g. [/company/index.md](https://github.com/flowforge/handbook/blob/main/company/index.md).

The `index.md` file can then have a `navTitle` at the top, which can define how that folder appears
in the navigation. It is also good practice to then add a manual table of contents for it's children
elements as seen in the `company/index.md` file linked above

If you are adding a top-level folder, e.g. `/development` or `/sales`, then it will need to have a
group defined too. Our current groups are:

- Company
- Development & Design Practices
- Internal Operations
- Sales & Marketing

If you add a new top-level folder, and do not define a group, it will appear in "Other".

To define a group for your folder, you can add a `navGroup` to the options at the top of the `index.md` file, e.g in `sales/index.md` we have:

    ---
    navGroup: Sales & Marketing
    ---