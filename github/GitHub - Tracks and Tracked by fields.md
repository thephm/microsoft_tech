---
tags:
  - git
---

# GitHub - Tracks and Tracked by fields

You can view the subtasks of the issues in your projects.

**Note:** Tasklists and the tracks and tracked by fields for Projects are currently in private beta and subject to change. If you are interested in trying tasklists and using the new fields, you can join the [waitlist](https://aka.ms/tasklist-roadmap-signup).

You can enable the Tracks and Tracked by fields on your projects to see the relationships between your issues as you add subtasks in tasklists. For more information about creating issue hierarchies in tasklists, see "[About tasklists](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-tasklists)."

The Tracked by field can be used to group items, creating a view that clearly shows the subtasks of each issue and the work required to complete them. For more information, see "[Changing the layout of a view](https://docs.github.com/en/issues/planning-and-tracking-with-projects/customizing-views-in-your-project/changing-the-layout-of-a-view#grouping-by-field-values-in-table-layout)."

You can also filter by the Tracked by field to display only items that are tracked by specific issues. Either start typing "tracked-by" and select an issue from the list or, if you know the repository and issue number, you can type the filter below in full.

```
tracked-by:"<OWNER>/<REPO>#<ISSUE NUMBER>"
```

To use the filter, replace `<OWNER>` with the repository owner, `<REPO>` with the repository name, and `<ISSUE NUMBER>` with the issue number. For more information, see "[Filtering projects](https://docs.github.com/en/issues/planning-and-tracking-with-projects/customizing-views-in-your-project/filtering-projects)."

## [Enabling the Tracked by field](https://docs.github.com/en/issues/planning-and-tracking-with-projects/understanding-fields/about-tracks-and-tracked-by-fields#enabling-the-tracked-by-field)

You can enable the Tracked by field to see which issues are tracking an item in your project.

1. In table view, in the rightmost field header, click .
    ![Screenshot showing new field button](https://docs.github.com/assets/cb-8051/images/help/projects-v2/new-field-button.png)
    
2. Under "Hidden fields", click **Tracked by**.
    
    ![Screenshot showing the field menu](https://docs.github.com/assets/cb-12274/images/help/projects-v2/select-tracked-by-field.png)

## [Enabling the Tracks field](https://docs.github.com/en/issues/planning-and-tracking-with-projects/understanding-fields/about-tracks-and-tracked-by-fields#enabling-the-tracks-field)

 Enable the `Tracks` field to see what other issues an item in your project is tracking.

1.  In table view, in the rightmost field header, click 
    
    ![Screenshot showing new field button](https://docs.github.com/assets/cb-8051/images/help/projects-v2/new-field-button.png)
    
2.  Under "Hidden fields", click **Tracks**.
    
    ![Screenshot showing the field menu](https://docs.github.com/assets/cb-12572/images/help/projects-v2/select-tracks-field.png)