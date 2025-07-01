# 相关资料

## file-system convention

<https://nextjs.org/docs/app/api-reference/file-conventions/layout#root-layouts>

## chapter 1

> why use Prisma

it automatically generates types based on your database schema.

## chapter 2 CSS Styling

### CSS module

CSS module allow you to scope CSS to a component by automatically create unique calss names, so you don't need to worry about style collisions as well.

Tailwind and CSS module are the two most common ways of styling Next.js applications.

#### using the clsx library to toggle class names

``` jsx
import clsx from 'clsx';
 
export default function InvoiceStatus({ status }: { status: string }) {
  return (
    <span
      className={clsx(
        'inline-flex items-center rounded-full px-2 py-1 text-sm',
        {
          'bg-gray-100 text-gray-500': status === 'pending',
          'bg-green-500 text-white': status === 'paid',
        },
      )}
    >
    // ...
)}
```

### other styling solutions

- CSS-in-JS libraries such as styled-jsx, styled-components

## chapter 3 optimizing Fonts and Images
