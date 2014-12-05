DirtyDataAlert
==============

One of the use case I recently encountered is to alert an user when he tries to close an kendo window and that kendo window has some dirty data in it’s kendo grid( user has edited the data in the kendo grid which is sitting on the kendo window).

I posted the working example @

http://jsfiddle.net/chandarmk/4ymkqL8L/

There are two extensions I have created

1. One is kendo.data.DataSource.prototype.isDirty which will let you know whether the datasource is dirty (whether user has altered data)

How to use it : just call dataSource.isDirty() which will return a Boolean indicating the status.

2. Second extension is kendo.ui.Window.prototype.enableConfirmChangesForGrid  while will alert the user about the dirty changes

How to use it: call kendowindo.enableConfirmChangesForGrid(modalGrid) – pass the kendo grid instance which is sitting on the kendo window to the method.

You can refer http://jsfiddle.net/chandarmk/4ymkqL8L/ for working demo
