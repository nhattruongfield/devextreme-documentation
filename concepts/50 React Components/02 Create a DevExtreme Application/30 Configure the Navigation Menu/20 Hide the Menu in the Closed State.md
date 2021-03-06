In the closed state, the navigation menu is partially visible because it displays item icons. If the items do not have icons, you can hide the menu. To do this, open the `SideNavOuterToolbar` or `SideNavInnerToolbar` component (depending on the used [layout](/Documentation/Guide/React_Components/Create_a_DevExtreme_Application/#Layouts)), find the [Drawer](/Documentation/ApiReference/UI_Widgets/dxDrawer/) configuration, and set its [minSize](/Documentation/ApiReference/UI_Widgets/dxDrawer/Configuration/#minSize) option to 0:

    <!-- tab: side-nav-outer-toolbar.js -->
    // ...
    export default function ({ title, children }) {
        // ...
        return (
            <div className={'side-nav-inner-toolbar'}>
                <Drawer ...
                    minSize={0}>
                    {/* ... */}
                </Drawer>
            </div>
        );
    }