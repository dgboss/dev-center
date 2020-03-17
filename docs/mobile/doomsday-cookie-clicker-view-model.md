```csharp
using App1.Components;
using Geocortex.Mobile.Composition;
using Geocortex.Mobile.Composition.Views;

[assembly: ViewModel(typeof(HarmlessComponentViewModel))]
namespace App1.Components
{
    public class HarmlessComponentViewModel : NotifyPropertyBase
    {
        private double _progress = 0;

        private bool _isDoomsday = false;

        public double Progress
        {
            get => _progress;
            set => SetProperty(ref _progress, value);
        }

        public bool IsDoomsday
        {
            get => _isDoomsday;
            set => SetProperty(ref _isDoomsday, value);
        }
    }
}

```