# libvideo

![icon](icons/icon_200.png)

## About 
libvideo (aka VideoLibrary) is a special .NET 1.4-compatible .NET library for downloading&playing YouTube videos. It is my attempt to return ability to play YT video via homemade retro apps such as YoutubeUWP or Windows 10 Mobile….

## Getting Started

Here's a small sample to help you get familiar with libvideo:

```csharp
using VideoLibrary;

void SaveVideoToDisk(string link)
{
    var youTube = YouTube.Default; // starting point for YouTube actions
    var video = youTube.GetVideo(link); // gets a Video object with info about the video
    File.WriteAllBytes(@"C:\" + video.FullName, video.GetBytes());
}
```

Or, if you use Visual Basic:

```vbnet
Imports VideoLibrary

Sub SaveVideoToDisk(ByVal link As String)
     Dim video = YouTube.Default.GetVideo(link)
     File.WriteAllBytes("C:\" & video.FullName, video.GetBytes())
End Sub
```

If you'd like to check out some more of our features, take a look at our [docs](docs/README.md). You can also refer to our [example application](samples/Valks/Valks/Program.cs) (named Valks, yes, I know, it's a silly name) if you're looking for a more comprehensive sample.

## License

libvideo is licensed under the [BSD 2-clause license](LICENSE).

## References
- https://github.com/omansak/libvideo Original project
- https://github.com/omansak OMANSAK, cool C# developer & main author of original libvideo 

## .
As is. No support. DIY. Learn purposes only.

## ..
[m][e] April 2025
