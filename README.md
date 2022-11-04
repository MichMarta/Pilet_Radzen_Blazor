# Pilet_Radzen_Blazor

This example try to build microfrontend with <a href="https://www.piral.io/">Piral</a>. The code is a <a href="https://learn.microsoft.com/en-us/aspnet/core/blazor/?view=aspnetcore-6.0">Blazor Webassembly</a> project, that uses the plugin <a href="https://github.com/smapiot/Piral.Blazor">Piral.Balzor</a> to create a pilet. The Blazor Project uses the NuGet Package <a href="https://blazor.radzen.com/">Radzen.Blazor</a> library to build a radzen form in Exmaple.razor.

The example is in this <a href="https://blazor.radzen.com/numericrangevalidator">page</a> and it is expected like this:
![expected](https://user-images.githubusercontent.com/50675825/200050586-f03d1e43-486c-404d-ac7a-5d8944253a3d.PNG)
<br/><br/><br/>
But the generated blazor pilet has no references to the static assets of Radzen.Blazor. The nomral Blazor wasm has references to these assests in index.html, as usual _content/Radzen.Blazor/Radzen.Blazor.js and _content/Radzen.Blazor/css/default-base.css. But these assets are missing in the pilet and this is the current behavior:
<br/><br/>
![what we get](https://user-images.githubusercontent.com/50675825/200053227-c1a75017-56eb-4805-8a3b-2e7b7d09e900.PNG)
![js missing](https://user-images.githubusercontent.com/50675825/200052479-6d106520-086b-4b5d-8687-9549a1a4b7bd.PNG)
