---
layout: default
permalink: index
---

<!-- hero !-->
<div class="layout-angle">
	<div class="top-triangle wow slideInRight" data-wow-duration="1.5s"></div>
	<div class="layout-angle-inner">
<div class="hero">
	<div class="container">
		<div class="row">
		
			<div class="col-lg-5 hero-header">
			
				<h1>
					<div class="display-4">Entity Framework Effort</div>
				</h1>
				
				<div class="wow zoomIn">
					<a class="btn btn-xl btn-z" href="{{ site.github.url }}/download"
							onclick="ga('send', 'event', { eventAction: 'download-hero'});">
						<i class="fa fa-cloud-download" aria-hidden="true"></i>
						NuGet Download
						<i class="fa fa-angle-right"></i>
					</a>
				</div>
				
				<div class="download-count">
					<div class="item-text">Download Count:</div>
					<div class="item-image wow lightSpeedIn"><img src="https://zzzprojects.github.io/images/nuget/entity-framework-effort-ef6-big-d.svg" /></div>
				</div>

				
			</div>
			
			<div class="col-lg-7 hero-examples">
			
				<div class="row hero-examples-1">
				
				
					<div class="col-lg-3 wow slideInUp"> 
						<h5 class="wow rollIn">EASY TO<br />USE</h5>
						<div class="hero-arrow hero-arrow-ltr">
							<img src="images/arrow-down1.png">
						</div>
					</div>

					<div class="col-lg-9 wow slideInRight">
						<div class="card card-code card-code-dark-inverse">
							<div class="card-header">Extend Entity Framework DbContext</div>
							<div class="card-body">
{% highlight csharp %}
// Returns categories stored in the database.
using(NorthwindEntities context = 
                            new NorthwindEntities())
{
    return context.Categories.ToList();
}

// Returns categories from in-memory database.
using(NorthwindEntities context = 
    Effort.ObjectContextFactory
        .CreateTransient<NorthwindEntities>())
{
    return context.Categories.ToList();
}
{% endhighlight %}
							</div>
						</div>
					</div>
				</div>
				<div class="row hero-examples-2">
				
					<div class="col-lg-3 order-lg-2 wow slideInDown">
						<h5 class="wow rollIn">EASY TO<br />CUSTOMIZE</h5>
						<div class="hero-arrow hero-arrow-rtl">
							<img src="images/arrow-down1.png">
						</div>
					</div>
					
					<div class="col-lg-9 order-lg-1 wow slideInLeft">
						<div class="card card-code card-code-dark-inverse">
							<div class="card-header">Flexible and feature-rich API</div>
							<div class="card-body">
{% highlight csharp %}
IDataLoader loader = 
    new EntityDataLoader("name=NorthwindEntities");
 
using(NorthwindEntities context = 
    ObjectContextFactory
        .CreateTransient<NorthwindEntities>(loader))
{
    return context.Categories.ToList();
}
{% endhighlight %}
							</div>
						</div>
					</div>						
				</div>
				
			</div>
		</div>
	</div>	
</div>
	</div>
	<div class="bottom-triangle-outer">
		<div class="bottom-triangle wow slideInLeft" data-wow-duration="1.5s"></div>
	</div>
</div>
<style>
.hero {
	background: transparent;
}
</style>


<!-- features !-->
<div class="features">

	<div class="container">
		
		<!-- more-feature !-->
		<div class="more">
			<a href="{{ site.github.url }}/tutorials" class="btn btn-z btn-xl" role="button">
				<i class="fa fa-book"></i>&nbsp;Read Tutorials
			</a>
		</div>
		
	</div>
</div>