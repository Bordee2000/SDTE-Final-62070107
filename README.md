# SDTE Final

## Flow
* **Login**

## Features
* **Login**
* Register
* confirmation

## Development Tool
* [Trello](https://trello.com/invite/b/dnLJxRjd/5d28258c8a7c2b423118a4bad60c7ab8/sdte-final)
* [Miro](https://miro.com/app/board/uXjVO2PtJzA=/?share_link_id=921411378269)

## Github
### Branch
* `Main` - When dev features that ready to be deployed on the production.
* `dev` - A develop branch for merging each feature branch.
* `feature/{feature name}` - For develop new features, eg: feature/a or feature/b.
* `debug/{feature name}` - For the feature that have to test something new or resolve the bug.

### Commit Message
Type of uses : 
```
<commit message> ...Refer To...
```
- `feature` - Use when some feature is created.
- `fix` - Use when some problem or bug is resolved.
- `add` - Use when add some function.
- `upd` - Use when want to improve some function.
- `del` - Use when some function or feature is deleted.
- `upl` - Use when some file is uploaded to Git except coding.

### Run Project
* Backend
```
cd backend
yarn install
node index.js
```
* Frontend
```
cd frontend
yarn install
yarn serve
```