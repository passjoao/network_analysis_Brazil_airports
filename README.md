# Brazilian flights and airports, case studies
- **Discipline**: IMD1155 - Network Analysis [![Open GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/ivanovitchm/network_analysis_2021)
- **Teacher**: Ivanovitch Medeiros Silva [![Open GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/ivanovitchm/)
- **author** João Victor Soares Oliveira [![Open GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/passjoao/)


## About
In this project, we used Álvaro F. P. P.'s [![Open GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/alvarofpp/) repository on Brazilian airports and their connections to conduct a study on the relationship between national airports and the behavior of each region using some measures seen in class. 5 exercises were created to analysis and measure their behavior.

let's go to them

## FIRST ANALYSIS
![image](https://user-images.githubusercontent.com/23378544/145103204-66bb84b5-b2b1-49e8-bd3e-46ce4d74f55a.png)

We need make a study on assortativity with the attribute region and make a similar graph of the assortativity

>we will use the circos graph by nxviz to perform a substantial analysis, checking if it has assortativity and the behavior of the relationships of each node

![image](https://user-images.githubusercontent.com/23378544/145103503-d8718e06-6663-423e-84f2-e1d4b2974218.png)
>This graph returns a positive assortativity coefficient for us, meaning that nodes tend to connect to nodes in the same region, but it is not a fully assortative network, as there are connections between different regions.

for better visualization, we will create the mixing matrix and heatmap to see the correlation between each region

![image](https://user-images.githubusercontent.com/23378544/145103937-46cdc1e4-792e-44b0-8f88-6bca0d951c3d.png)
>As stated, each region tends to connect with itself, observed by the main diagonal, highlighting the southeast and north with the warmer regions. it is worth mentioning the relationship between north and south that almost does not exist

## SECOND ANALYSIS
![image](https://user-images.githubusercontent.com/23378544/145104279-3f17b60e-b5e5-4a1c-935f-afaad79561dc.png)
 
To make the Bivariate analysis, we will use the Scatter plot and the regression plot between node degree and average neigbhor degree of the country and each region.

The assortativity coefficient can show us whether the behavior of the network is assortative or dissortative (i.e core nodes try to connect with other core nodes or with leaf nodes). If the assortativity coefficient is between 0 and 1 is assortative, else is dissortative

>Let's make firts for the country

![image](https://user-images.githubusercontent.com/23378544/145104386-f48f13c1-c492-45a3-b7e9-b9a9ef24c3a3.png)
>we can observe that it has a certain drop, indicating a disassortative analysis, but for a better analysis, let's see the behavior in each region.

>To the north

![Assortativity between node degree and average neighbor degree - North region](https://user-images.githubusercontent.com/23378544/145104784-b063566b-1fd4-4d7b-9847-8a507d779ff2.png)

>To the northeast


![image](https://user-images.githubusercontent.com/23378544/145104999-c967fbf7-617f-4865-9df2-75befe1d3070.png)

>To the midwest


![image](https://user-images.githubusercontent.com/23378544/145105054-cc5b2d0b-14f9-403f-8f9e-03cba99520df.png)

>To the shoutheast


![image](https://user-images.githubusercontent.com/23378544/145105102-82b45d91-ceb9-4ece-b5cd-c7c2f374f4fc.png)

>And to the south


>![image](https://user-images.githubusercontent.com/23378544/145105163-61100d27-3a21-4ac6-b0d8-715081483607.png)


**Conclusion**

this network has disassortative characteristics according to the coefficients obtained in each region and in the entire country, i.e, the central nodes tend to connect with the leaves and the opposite happens


## TIRD ANALYSIS

![image](https://user-images.githubusercontent.com/23378544/145105401-c8ecf5cd-cef6-4488-9a0f-d0f18e7943c6.png)

On this step, we need see the components connected in the aerial network, characterized by quantity, percentage per region

>![image](https://user-images.githubusercontent.com/23378544/145105489-84199d31-d8ae-47de-be38-2e5e897ab2a3.png)
 
 
The GCC (Giant Connected Component) contains 491 connected airports and the other networks are individual nodes
<p>

*note*: SNBG, SSBE, SNGR and SBER airports are small airports, operating under VFR (Visual Flight rules) and runways smaller than 2000 meters and do not have a structure to receive medium and large aircraft from airlines, thus being separated from the large network <small>(data obtained by the flightmarket website)

---
to get the percentage per region we will get only de region from the GCC
  
![image](https://user-images.githubusercontent.com/23378544/145105733-2778ce7b-516e-410e-b003-00f8042cc068.png)
>In GCC, the most airports aer in north region with 25,6619% and the less is in south with 14,2566%
  
  
## FOURTH ANALYSIS
![image](https://user-images.githubusercontent.com/23378544/145105804-c150e5ae-2394-4356-b1de-abd4e2bd2c35.png)
  
we need to travel using airports from different regions, going from the north to the south, then to the northeast then to the midwest and finally to the south

---

So, for our scenario, imagine that João needs to travel from Manaús/AM to Porto Alegre/RS to take an entrance exam, then he goes to Natal/RN to visit a distant relative, and then goes to the Federal District to get a passport visa to a foreign country and then goes to São Paulo/SP to participate in a job interview at a multinational

![image](https://user-images.githubusercontent.com/23378544/145105945-c213c5a0-bfbe-43f1-b1c5-7a74461f8516.png)
![image](https://user-images.githubusercontent.com/23378544/145106246-6940d810-166d-4597-b1ba-71e09026ae85.png)
![image](https://user-images.githubusercontent.com/23378544/145105985-2cfa41d2-c5ab-4290-90fa-de5ee8b2fc5f.png)
![image](https://user-images.githubusercontent.com/23378544/145106031-08e54cac-3b45-4305-bbb2-d2aa7b3873bd.png)
![image](https://user-images.githubusercontent.com/23378544/145106050-7388115c-e36d-46b8-9854-d75151dd6cba.png)

I randomly chose locations, but all trips were between direct flights in each city.😢
  
## FIFTH ANALYSIS
![image](https://user-images.githubusercontent.com/23378544/145106330-e3315d37-1a7c-4ec9-9a86-049f4f2f6c09.png)

by definition, Clustering coefficient is a measure of the degree to which nodes in a graph tend to cluster together.
So, let's use the Clustering function networkx to measure Brazil and each region
  
>first see the average of clustering of the graph
  ![image](https://user-images.githubusercontent.com/23378544/145106440-c344506e-a87e-492c-ab38-2fecf837b432.png)
  >that means we have a high level of clustering

**Conclusion**  

![image](https://user-images.githubusercontent.com/23378544/145106564-a1bd75eb-5396-4642-8ac7-734ddd2ab8b1.png)
  >Looking across all regions, we have at least one fully clustered airport
  
now looking at the big picture, we see that we have several airports completely clustered.
<p>
![image](https://user-images.githubusercontent.com/23378544/145107171-fb2fbdf9-37f2-478c-a483-4101b92fa09b.png)

  
  

