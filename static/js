var tableData = data;

tablebody = d3.select("tbody")


function createTable(data){ 
    tbody.text(" ")
    data.forEach(function(ufoInfo){
    var row = tbody.append("tr")
    Object.entries(ufoInfo).forEach(function([key, value]){
        row.append("td").text(value)	
    })
})}

createTable(tableData);

var submit = d3.select("#filter-btn");

submit.on("click", function() {
  d3.event.preventDefault();
  var occurenceDate = d3.select("#datetime");
  console.log("The date of the UFO sighting is");
  console.log(occurenceDate.property("value"));
  var filteredData = tableData.filter(ufoInfo => ufoInfo.datetime === occurenceDate.property("value"));

createTable(filteredData)
occurenceDate.on("change", filterDate)
});
