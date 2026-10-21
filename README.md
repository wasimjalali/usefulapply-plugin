# Useful Apply for Claude Code

Prepare job applications from Claude Code. This plugin connects Claude Code to your Useful Apply account and adds one skill, `apply-to-job`, that walks through a full application: fit check, tailored CV, cover letter and emails, export and tracking.

Nothing is ever submitted to an employer. The plugin drafts your documents and you apply yourself.

It's a plugin and its own marketplace.

## Install

```
/plugin marketplace add wasimjalali/usefulapply-plugin
/plugin install usefulapply@usefulapply
```

## Sign in

The first time Claude calls a Useful Apply tool, your browser opens and you sign in to Useful Apply with OAuth. No keys go in any file. You approve up to three scopes:

- **Read**: see your account, credits, CVs and applications.
- **Edit**: change your applications, CVs and profile. Costs no credits.
- **Spend credits**: start work that uses your credits, up to your daily agent limit.

You can revoke access any time under Settings > Connected apps in Useful Apply.

## What the skill does

`apply-to-job` runs the workflow in order and asks before it spends anything:

1. Checks your account and CV.
2. Creates the application from the job ad.
3. Runs a fit check.
4. Shows the fit and asks whether to generate.
5. Generates the kit and waits for it.
6. Reviews the result with you.
7. Exports PDFs and other files.
8. Sets the tracker status and dates.

Edits to your CV and letters use your own words. AI rewrites only run when you ask.

## Tools

**Read**
`get_account`, `get_credit_history`, `list_applications`, `get_application`, `get_operation`, `get_cv`, `get_cv_outline`, `list_cv_templates`, `get_job_feed`, `get_feed_settings`, `get_career_profile`, `explain_fit`, `morning_briefing`

**Spend credits**
`analyze_job_fit`, `generate_application_kit`, `regenerate_document`, `rewrite_cv_section`, `apply_to_feed_job`, `draft_screening_answers`

`draft_screening_answers` costs no credits. It uses one of an application's limited screening turns and needs a plan that includes screening answers.

**Free writes**
`create_application`, `update_application`, `update_application_status`, `delete_application`, `cancel_generation`, `save_cv`, `delete_cv`, `set_profile_photo`, `remove_profile_photo`, `update_profile`, `update_cv_content`, `add_cv_item`, `set_cv_item_visibility`, `undo_last_edit`, `edit_cv_structure`, `delete_cv_item`, `edit_document_text`, `set_cv_template`, `export_documents`, `run_job_feed`, `update_feed_settings`, `give_job_feedback`, `withdraw_feed_consent`, `update_notification_settings`

## Privacy, terms and support

- Privacy: https://usefulapply.com/privacy
- Terms: https://usefulapply.com/terms
- Support: support@usefulapply.com or https://usefulapply.com/integrations

## License

MIT
