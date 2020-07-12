<template>
   <main class="col-lg-9" >
        <nav aria-label="breadcrumb">
            <ol class="breadcrumb">
                <li class="breadcrumb-item"><a href="#">Home</a></li>
                <li class="breadcrumb-item"><a href="#">Library</a></li>
                <li class="breadcrumb-item active" aria-current="page">Data</li>
            </ol>
        </nav>

       <h1>Main H1</h1>

       <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam id eveniet sit nulla cumque non nobis modi ipsa nostrum cupiditate saepe fuga totam quidem, quia culpa provident quod suscipit assumenda.</p>
       <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Maxime neque exercitationem nisi amet laboriosam quia obcaecati reiciendis incidunt, dolore error suscipit aliquid. Distinctio qui officiis perferendis libero, aut nihil nemo deleniti quam aspernatur, rerum accusantium nam iste? Repellat nam ullam soluta illo repudiandae maiores, perspiciatis ipsum velit minus, vero voluptates!</p>

        <ul class="nav nav-tabs" id="myTab" role="tablist">
            <li class="nav-item" role="presentation">
                <a class="nav-link active" id="home-tab" data-toggle="tab" href="#home" role="tab" aria-controls="home" aria-selected="true">Home</a>
            </li>
            <li class="nav-item" role="presentation">
                <a class="nav-link" id="profile-tab" data-toggle="tab" href="#profile" role="tab" aria-controls="profile" aria-selected="false">Profile</a>
            </li>
            <li class="nav-item" role="presentation">
                <a class="nav-link" id="contact-tab" data-toggle="tab" href="#contact" role="tab" aria-controls="contact" aria-selected="false">Contact</a>
            </li>
        </ul>
        <div class="tab-content mb-1" id="myTabContent">
            <div class="tab-pane p-3 fade show active" id="home" role="tabpanel" aria-labelledby="home-tab">Text1</div>
            <div class="tab-pane p-3 fade" id="profile" role="tabpanel" aria-labelledby="profile-tab">Text2</div>
            <div class="tab-pane p-3 fade" id="contact" role="tabpanel" aria-labelledby="contact-tab">Text3</div>
        </div>

       <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptatum sunt quae consequatur eius, dolor consequuntur impedit tempora eaque dolore, repellat commodi assumenda! Eligendi dolorem nemo enim consequuntur aut, doloribus accusantium officiis saepe. Earum autem necessitatibus consequatur, placeat unde totam rerum veritatis voluptates, aliquid vero nulla animi esse natus eligendi quaerat, eius assumenda officiis? Labore laudantium velit asperiores error magni unde repudiandae voluptates alias dolores iusto hic qui explicabo, ab modi ex deserunt iste eligendi sequi mollitia impedit tempora aliquid. Totam, tempore necessitatibus! Excepturi quaerat deserunt laudantium magni nostrum rem! Facilis explicabo beatae, veniam vero eaque asperiores neque quas optio aperiam?</p>

    <div class="accordion" id="accordionExample">
    <div class="card">
        <div class="card-header" id="headingOne">
        <h2 class="mb-0">
            <button class="btn btn-link btn-block text-left shadow-none" type="button" data-toggle="collapse" data-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
            Collapsible Group Item #1
            </button>
        </h2>
        </div>

        <div id="collapseOne" class="collapse show" aria-labelledby="headingOne" data-parent="#accordionExample">
            <div class="card-body">
                Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic synth nesciunt you probably haven't heard of them accusamus labore sustainable VHS.
            </div>
            </div>
        </div>
        <div class="card">
            <div class="card-header" id="headingTwo">
            <h2 class="mb-0">
                <button class="btn btn-link btn-block text-left shadow-none collapsed" type="button" data-toggle="collapse" data-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
                Collapsible Group Item #2
                </button>
            </h2>
            </div>
            <div id="collapseTwo" class="collapse" aria-labelledby="headingTwo" data-parent="#accordionExample">
            <div class="card-body">
                Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic synth nesciunt you probably haven't heard of them accusamus labore sustainable VHS.
            </div>
            </div>
        </div>
        <div class="card">
            <div class="card-header" id="headingThree">
            <h2 class="mb-0">
                <button class="btn btn-link btn-block text-left shadow-none collapsed" type="button" data-toggle="collapse" data-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
                Collapsible Group Item #3
                </button>
            </h2>
            </div>
            <div id="collapseThree" class="collapse" aria-labelledby="headingThree" data-parent="#accordionExample">
            <div class="card-body">
                Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic synth nesciunt you probably haven't heard of them accusamus labore sustainable VHS.
            </div>
            </div>
        </div>
    </div>
       
   </main>
</template>

<script>
export default {
  data() {
      return {
      }
  }
}
</script>

<style>
</style>
