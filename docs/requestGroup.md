# Request group

There are groups of requests for easy grouping and request browsing. Each request is tied to a group. Groups can be as many as you like and each group can have as many requests as possible.

For example, the group structure may look like this:

```text
└── Request groups
    ├── Group for POST requests
        ├── POST 1
        └── POST 2
    ├── Group for GET requests
      ├── GET 1
    └── Group for PUT requests
        ├── PUT 1
        └── PUT 2
        ├── PUT 3
        └── PUT 4
```

## Creating

To create a group, select the `Organization administration` module, then `Ax Change` and in the list open the `Request group` form.

![](../_media/requestGroup_1.png ":size=300x450")

## Filling

To successfully create a group, you must fill in the field `Group Name`.

> The `Data source name` field must be filled in according to the`Only for internal` setting. If it is in the `No`, then the field is required to fill.

The Description field is optional.

| Field             | Required                                                                                   | Description                                                                                                            |
| ----------------- | ------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------- |
| Group name        | <code>Yes</code>                                                                           | Name of request group                                                                                                  |
| Description       | <code>No</code>                                                                            | Description of the request group                                                                                       |
| Only for internal | <code>No</code>                                                                            | Only for internal use only, so this record cannot be related to the system entity. Group does not contain data sources |
| Data source name  | <code>No</code> if `Only for internal` set to <code>Yes</code>, otherwise <code>Yes</code> | The main data source for all requests in this group                                                                    |

> When changing the `Only for internal` parameter, the value in the`Data source name` field is cleared.

Also, button `Request parameter` is present on the form by clicking on which you can go to the requests associated with the group. More about requests in the [Request parameter](requestParameter.md).

![](../_media/requestGroup_2.png)
