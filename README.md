# Xamarin.Forms-CardView
A Package to create a CardView using Xamarin.Forms that works on the three platforms (Android, iOS, UWP)
It is simple to use in a straight forward fashion.
You may either use it in C#, or in XAML.  

---
To Install this nuget package:
> PM> Install-Package XamarinForms.CardView
---

## CardView Bindable Properties

| Property                              		  | Property Name                 		    | Property Type   | Usage           		 			  | Default Value   |
| :-------------:                       		  | :-------------:               		    | :-------------: | :-------------: 		 			  | :-------------: |
| CardViewContentProperty               		  | CardViewContent               		    | View            | CardView Content 		 			  | None            |
| CardViewHeightRequestProperty         		  | CardViewHeightRequest                   | double          | Height Request  		 		 	  | 300.0           |
| CardViewOutlineColorProperty          		  | CardViewOutlineColor                    | Color           | Outline Color   		 			  | Transparent     |
| CardViewInnerFrameOutlineColorProperty 		  | CardViewInnerFrameOutlineColor          | Color 		  | Inner OutlineColor 					  | Transparent 	|
| CardViewOutlineColorThicknessProperty 		  | CardViewOutlineColorThickness           | Thickness       | OutlineColor Thickness   			  | 0    		    |
| CardViewInnerFrameOutlineColorThicknessProperty | CardViewInnerFrameOutlineColorThickness | Thickness 	  | Inner OutlineColor Thickness 		  | 0 				|
| CardViewHasShadowProperty 					  | CardViewHasShadow 						| bool            | Card View Shadow 					  | false           |  
| IsSwipeToClearEnabledProperty          		  | IsSwipeToClearEnabled          			| bool       	  | Enable to clear Content With a Swipe  |  false          |

### CardViewContent Example:  

```xml
	<CardView>
		<CardView.CardViewContent>
			<StackLayout>
				<Label Text="Label inside StackLayout forming the CardViewContent"></Label>
			</StackLayout>
		</CardView.CardViewContent>
	</CardView>
```

### CardViewHeightRequest Example:  

```xml
	<cardView:CardView CardViewHeightRequest="100">
		<cardView:CardView.CardViewContent>
			<StackLayout>
				<Label Text="I have 100 Height"></Label>
			</StackLayout>
		</cardView:CardView.CardViewContent>
	</cardView:CardView>
```

### CardViewOutlineColor Example:  

```xml
	<cardView:CardView CardViewHeightRequest="100" CardViewOutlineColor="Black" CardViewOutlineColorThickness="2">
		<cardView:CardView.CardViewContent>
			<StackLayout  BackgroundColor="White">
				<Label Text="I have 100 HeightRequest, and a black outline color"></Label>
			</StackLayout>
		</cardView:CardView.CardViewContent>
	</cardView:CardView>
```

### CardViewInnerFrameOutlineColor Example:  

```xml
	<cardView:CardView CardViewHeightRequest="100" CardViewOutlineColor="Black" CardViewOutlineColorThickness="2"
				   CardViewInnerFrameOutlineColor="Aqua" CardViewInnerFrameOutlineColorThickness="2">
		<cardView:CardView.CardViewContent>
			<StackLayout  BackgroundColor="White">
				<Label Text="I have 100 Height, and a black outline color, and an inline outline color Aqua"></Label>
			</StackLayout>
		</cardView:CardView.CardViewContent>
	</cardView:CardView>
```

### CardViewHasShadow Example:  

```xml
	<cardView:CardView CardViewHeightRequest="100" CardViewOutlineColor="Gray" CardViewOutlineColorThickness="2" CardViewHasShadow="True">
		<cardView:CardView.CardViewContent>
			<StackLayout  BackgroundColor="White">
				<Label Text="Gray Outline Color with Shadow"></Label>
			</StackLayout>
		</cardView:CardView.CardViewContent>
	</cardView:CardView>
```

### IsSwipeToClearEnabled Example:  

```xml
	<cardView:CardView CardViewHeightRequest="100" CardViewOutlineColor="Gray" CardViewOutlineColorThickness="2" CardViewHasShadow="True"
						   IsSwipeToClearEnabled="True">
		<cardView:CardView.CardViewContent>
			<StackLayout  BackgroundColor="White">
				<Label Text="Swipe me and I will go away"></Label>
			</StackLayout>
		</cardView:CardView.CardViewContent>
	</cardView:CardView>
```

