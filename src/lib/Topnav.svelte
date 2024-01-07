<script lang="ts">
	import { base } from '$app/paths';
    import {
        Navbar,
        Collapse,
        Nav,
        NavItem,
		NavbarBrand,
        NavbarToggler,
        Dropdown,
        DropdownItem,
        DropdownToggle,
        DropdownMenu,
        NavLink,

    } from '@sveltestrap/sveltestrap';

    let isOpen = false;
</script>

<Navbar
    sticky="top"
    color="dark-subtle"
    light
    expand="md"
>
    <NavbarBrand href="{base}/">KWR-Informatik-AG</NavbarBrand>
    <NavbarToggler on:click={() => (isOpen = !isOpen)}/>
    <Collapse {isOpen} navbar expand="md">
        <Nav class="ms-auto" navbar>
            <NavItem>
                <NavLink
                    href="https://kwr-informatik-ag.github.io/learn/"
                    target="_self"
                ></NavLink>
            </NavItem>
            <!--<NavItem>
                <NavLink
                    href="https://kwr-hannover.de/"
                    target="_self"
                >Hauptseite</NavLink>
            </NavItem>-->
            <NavItem>
                <NavLink
                    href="https://kwr-informatik-ag.github.io/documentation/"
                    target="_self"
                >Dokumentation</NavLink>
            </NavItem>
        </Nav>
    </Collapse>
</Navbar>