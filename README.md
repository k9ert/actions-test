# actions-test

# Trigger Tag Creation

In order to trigger the repo_dispatch_event of type `create-tag` do this:

```
export REPO_DISPATCH_TEST=ghp_wZ...
curl -X POST \                                                    
  -H "Authorization: token $REPO_DISPATCH_TEST" \
  -H "Accept: application/vnd.github.v3+json" \
  https://api.github.com/repos/k9ert/actions-test/dispatches \
  -d '{"event_type": "create-tag"}'
```
