# clerk-shadcn-theme
Easily synchronize your Clerk Sign-in and Sign-up components with your Shadcn styles using the provided CSS styles.

![Screenshot_4](https://github.com/stormynight9/clerk-shadcn-theme/assets/81434423/65804b03-cf66-43e0-ab19-9158c6ecf003)

1. Configure your primary color:
```jsx
<ClerkProvider
    appearance={{
        variables: {
            colorPrimary: 'hsl(263.4, 70%, 50.4%)', // change this value (you can get it from you're css variables, make sure to include 'hsl' and commas)
                },
            }}
>
...
</ClerkProvider>
```

2. Copy and paste the following code into your global CSS file, and you're good to go!
```css
.cl-formButtonPrimary {
    @apply inline-flex h-9 items-center justify-center whitespace-nowrap rounded-md bg-primary px-3 text-xs font-medium text-primary-foreground ring-offset-background transition-colors hover:bg-primary/90 focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50;
}

.cl-card,
.cl-socialButtonsBlockButton,
.cl-alert,
.cl-identityPreview,
.cl-phoneInputBox,
.cl-userButtonPopoverCard {
    @apply border border-input bg-background;
}

.cl-headerTitle,
.cl-socialButtonsBlockButtonText,
.cl-loading,
.cl-formFieldLabel,
.cl-formHeaderTitle,
.cl-selectButton__countryCode,
.cl-selectButton__countryCode p,
.cl-selectOption p,
.cl-selectOption div,
.cl-modalCloseButton,
.cl-navbarButton,
.cl-breadcrumbsItem.cl-breadcrumbsItem__currentPage,
.cl-profileSectionTitle p,
.cl-userPreviewTextContainer,
.cl-profileSectionContent p,
.cl-form p,
.cl-accordionTriggerButton {
    @apply dark:text-foreground;
}

.cl-headerSubtitle,
.cl-dividerText,
.cl-footerActionText,
.cl-alertText,
.cl-formFieldInfoText,
.cl-formFieldSuccessText,
.cl-identityPreviewText,
.cl-userButtonPopoverActionButton,
.cl-userButtonPopoverActionButton svg,
.cl-userButtonPopoverActionButtonText,
.cl-userButtonPopoverFooter p,
.cl-userButtonPopoverFooter a,
.cl-formHeaderSubtitle,
.cl-breadcrumbsItem,
.cl-breadcrumbsItemDivider,
.cl-fileDropAreaHint,
.cl-fileDropAreaFooterHint,
.cl-form
    p[data-localization-key='userProfile.emailAddressPage.emailCode.formHint'],
p[data-localization-key='userProfile.profilePage.successMessage'] {
    @apply text-muted-foreground;
}

.cl-dividerLine {
    @apply bg-border;
}

.cl-formFieldInput[type='text'],
.cl-formFieldInput[type='email'],
.cl-formFieldInput[type='password'] {
    @apply flex h-10 w-full rounded-md border border-input bg-background px-3 py-2 text-foreground ring-offset-background file:border-0 file:bg-transparent file:text-sm file:font-medium placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:cursor-not-allowed disabled:opacity-50;
}

.cl-footerActionLink {
    @apply text-accent-foreground underline hover:text-accent-foreground/90;
}

.cl-otpCodeFieldInput {
    @apply border border-b-input text-foreground;
}

.cl-formResendCodeLink {
    @apply text-primary disabled:opacity-90;
}

.cl-selectSearchInput__countryCode {
    @apply flex h-10 w-full rounded-md border border-b border-input bg-background text-foreground ring-offset-background file:border-0 file:bg-transparent file:text-sm file:font-medium placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:cursor-not-allowed disabled:opacity-50;
}

.cl-selectOptionsContainer__countryCode {
    @apply border border-input bg-background;
}

.cl-internal-icon,
.cl-userPreviewSecondaryIdentifier__userButton {
    @apply text-foreground;
}

.cl-profileSectionTitle {
    @apply border-b border-input;
}

button[data-localization-key='userProfile.start.dangerSection.deleteAccountButton'] {
    @apply bg-destructive text-destructive-foreground hover:bg-destructive/90;
}

.cl-fileDropAreaBox {
    @apply dark:bg-gray-900;
}

.cl-fileDropAreaIconBox {
    @apply dark:bg-gray-800;
}

.cl-fileDropAreaIcon {
    @apply dark:text-gray-400;
}

.cl-fileDropAreaButtonPrimary {
    @apply h-10 px-4 py-2 text-foreground transition-colors hover:bg-secondary hover:text-accent-foreground;
}

.cl-userButtonPopoverActionButton,
.cl-profileSectionPrimaryButton,
.cl-accordionTriggerButton,
.cl-navbarButton {
    @apply hover:bg-accent hover:text-accent-foreground;
}

.cl-card {
    @apply rounded-lg shadow-md;
}

.cl-userButtonPopoverCard {
    @apply rounded-md;
}

.cl-userButtonPopoverFooter a {
    @apply hover:text-muted-foreground;
}

.cl-badge {
    @apply rounded-full px-2.5 py-0.5 text-xs;
}

.cl-badge[data-localization-key='badge__unverified'] {
    @apply border bg-transparent text-destructive dark:text-red-500;
}

.cl-formButtonReset {
    @apply text-foreground hover:bg-secondary;
}


```
