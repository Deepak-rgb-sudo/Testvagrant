# Testvagrant
Code
validate 4 foreign player
RestAssured.baseURI="";

String response=
given().body(),
when().("Resource"),
then().statuscode(200).extract().asString();

JsonPath jpath = new JsonPath(response);
int roleCount=jPath.getInt("player.role");

for(int i=0; i<=roleCount; i++)
{
if(jPath.getString(player.country)!="India")
{
int countFP=i;
}
}

Assert.assertEquals(countFP,4);



validate at least 1 wicketkeeper

RestAssured.baseURI="";
String response=
RestAssured.given().body(),
when().("Resource"),
then().statuscode(200).extract().asString();

JsonPath jpath = new JsonPath(response);
int roleCount=jPath.getInt("player.role");

for(int i=0; i<=roleCount; i++)
{
if(jPath.getString(player.role).EqualsIgnoreCase("Wicket-keeper")
{
System.out.println("Wicket-keeper found");
break;
}
}

Assert.assertEquals(roleCount,"WiketKeeper");
