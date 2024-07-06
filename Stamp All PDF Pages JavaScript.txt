this.syncAnnotScan();
var annt = this.getAnnots(this.pageNum)[0];
var props = annt.getProps();
for(var i=0;i<this.numPages;i++){
props.page = i;
if(i !=this.pageNum)
this.addAnnot(props);
}