#Change log

##2.0.15 - 2016-12-31
- Pages: 
    + Add CreatePageRequest
    + Fix bugs pages list cannot use group actions
    + Add PagesListDataTable to filter pages.index.get, datatables.pages.index.post
    + Rename EloquentPage to Page
- ACL
    + Add field created_by, updated_by, timestamps to table roles
    + Separate create and update roles into 2 method
    + Rename model EloquentPermission to Permission, EloquentRole to Role
    + Use form request to update/create roles
    + Save author and modifier when update/create roles
    + Rename RoleContract to RoleRepositoryContract, PermissionContract to PermissionRepositoryContract
    + Refactor
- Menus:
    + Separate create/update method      
    + Add target field
    + Use form request
    + Refactor
- Users:
    + Rename UserContract to UserRepositoryContract
    + Rename EloquentUser to User
    + Add form request
    + Use soft deletes
    + Refactor
- Base:
    + Add soft deletes to repositories
- Caching:
    + Add soft deletes repositories cache

##2.0.14 - 2016-12-27
- Refactor data table renderer.
- Add hook filter before edit, delete (pages, menus).

##2.0.13 - 2016-12-19
- Caching: remove magic method __call in AbstractRepositoryCacheDecorator

##2.0.13 - 2016-12-18
###Modify
- Add cors

##2.0.12 - 2016-12-18
###Modify
- Add class Constants to manage const
- Add SEO helper
- Add CKeditor to WebEd core js
- Refactor
- Remove unused files
- Add version
- Users: Add birthday, description, disabled_until to fillable
- Shortcode: Add helper generate_shortcode
- Caching: Add cache lifetime to env
- Pages: Fix bugs when create page, Pass seo data to front site
- ACL: Order permissions by namespace
- Refactor routes middleware


##2.0.11 - 2016-12-13
###Modify
- Travis CI test: cms:install
- phpunit.xml config
- Remove themes folder. Please get themes from [WebEd themes](https://github.com/webed-themes/readme)

##2.0.11 - 2016-12-12
###Added
- Travis CI test: cms:install
- Travis CI config