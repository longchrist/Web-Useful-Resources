# Web Useful Resources
web programming useful resources link

berikut adalah link yang penting :<br/>
# CSS / Font Graphics
Web Icon-Fonts Graphics :<br/>
1. <a href="http://glyphicons.com/" target="_blank">Glyphicons Icons</a><br/>
2. <a href="https://fortawesome.github.io/Font-Awesome/icons/" target="_blank">Font-Awesome Icons</a><br/>

# Javascript / Client Side
Javascript Modules :<br/>
1. <a href="http://wenzhixin.net.cn/p/multiple-select/docs/" target="_blank">Multiple Select</a><br/>
Info ajax<br/>
```javascript
  $.ajax(
        url 		: 'functions_link.php',
		type 		: 'POST',
		data 		: JSON.stringify(getDataFunctions()),
		success		: function(response) {resultData(response)},
		error		: function(e) {onError(e);},
		dataType 	: 'json',
		contentType : 'application/json'
	});
```
Info ajax File Upload<br/>
```javascript
  $.ajaxFileUpload({
		url 			: 'functions_link.php',
		type 			: 'POST',
		secureuri      	: false,
		fileElementId	: 'temporary_image',
		data			: JSON.stringify(data),
		success			: function(response) {resultUpload(response);},
		error			: function(e) {onError(e);},
		dataType 		: 'json'
	});
```
# PHP Framework
PHP Framework :<br/>
1. <a href="https://github.com/ivantcholakov/starter-public-edition-3" target="_blank">Code-Igniter 3</a><br/>

# Web Programming Tutorials
1. <a href="http://www.w3schools.com/" target="_blank">w3schools</a><br/>
2. <a href="http://www.javatpoint.com/" target="_blank">Java Web Services Tutorial 1</a><br/>
3. <a href="http://docs.oracle.com/javaee/6/tutorial/doc/gijti.html" target="_blank">Oracle Introduction to Web Services - Java EE 6</a><br/> 

# JavaEE Web Services
1. <a href="https://docs.oracle.com/javaee/6/tutorial/doc/giepu.html" target="_blank">Building RESTful Web Services with JAX-RS</a><br/>
2. 

Simple Java RESTful WebService Function Example<br/>
```java
    @GET
    @Path("Barcode/{Barcodes}")
    @Produces("text/plain")
    public String getValues(@PathParam("Barcodes") String BarCD) {

        String Bar_code = "";
        String ValueHarga = "";
        String NamaBar = "";
        String Stat = "";
        String Parameters = BarCD;

        Statement stmt = null;
        ResultSet rs;
        String _DB_URL = "jdbc:mysql://localhost:3306/<db_name>";
        String _DB_USERNAME = "<db_username>";
        String _DB_PASSWORD = "<db_password>";

        try {
            Class.forName("com.mysql.jdbc.Driver");
            conn = (Connection) DriverManager.getConnection(_DB_URL, _DB_USERNAME, _DB_PASSWORD);
            stmt = conn.createStatement();
            String query = "SELECT tb_data2.barcode, tb_data2.valuesHarga, tb_data2.namaBarang, tb_data2.STATUS FROM tb_data2 WHERE barcode = '" + Parameters + "';";
            rs = stmt.executeQuery(query);
            while (rs.next()) {
                Bar_code = rs.getString("barcode");
                ValueHarga = rs.getString("valuesHarga");
                NamaBar = rs.getString("namaBarang");
                Stat = rs.getString("STATUS");
            }

        } catch (Exception e) {
            e.printStackTrace();
        }
        return "RESTful WebService Response :\n - Bar-Code : " + Bar_code + "\n - Nama Barang : " + NamaBar + "\n - Harga Barang : " + ValueHarga + "\n - Data Status : " + Stat;
    }
```

# Community
PHP Indonesia : <br/>
PHP Indonesia Official Link : <a href="http://www.phpindonesia.or.id/" target="_blank">Official</a><br/>
PHP Indonesia Facebook Link : <a href="https://www.facebook.com/groups/35688476100/10153668442436101/" target="_blank">Facebook</a><br/>
